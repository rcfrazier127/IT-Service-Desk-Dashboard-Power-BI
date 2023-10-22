# IT-Service-Desk-Dashboard

(Under Construction)

<img width="900" alt="image" src="https://github.com/rcfrazier127/IT-Service-Desk-Dashboard/assets/63532077/69dc432e-ff20-4e7c-a728-da421d7bedf8">

<img width="1180" alt="image" src="https://github.com/rcfrazier127/IT-Service-Desk-Dashboard/assets/63532077/c9159583-f670-484b-915a-caa8a52ff3ed">

<img width="1575" alt="image" src="https://github.com/rcfrazier127/IT-Service-Desk-Dashboard/assets/63532077/6033614b-9a9a-45ff-b03e-090e6cb5a6c0">

= Table.AddColumn(#"Reordered Columns", "Time Buckets", each if [Days Open] >= 0 and [Days Open] <= 5 then "0-5 days"
else if [Days Open] >= 6 and [Days Open] <= 10 then "6-10 days"
else if [Days Open] >= 11 and [Days Open] <= 15 then "11-15 days"
else if [Days Open] >= 16 and [Days Open] <= 20 then "16-20 days"
else if [Days Open] >= 21 and [Days Open] <= 25 then "21-25 days"
else if [Days Open] >= 26 and [Days Open] <= 37 then "25+ days"
else "More than 37 days")
