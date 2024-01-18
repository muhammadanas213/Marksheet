# Marksheet
students_data = [  
                    ("ahmed","ali","34","65","73"),
                    ("noman","haider","72","56","76"),
                    ("owais","qazi","62","81","91"),
                    ("javed","ali","91","83","72"),
                    ("khalid","azeem","76","52","72"),
                    ("usman","arif","75","63","43"),
                ]
total_marks = 300
passing_marks = 50
for data in students_data:
    name = data[0]
    fname = data[1]
    maths_marks = int(data[2])
    physics_marks = int(data[3])
    sindhi_marks = int(data[4])
    total_marks_obtained = sum([maths_marks,physics_marks,sindhi_marks])
    percentage =(total_marks_obtained*100)/ total_marks
    if maths_marks >= passing_marks and physics_marks >= passing_marks and sindhi_marks  >= passing_marks:
        result = "passed"
    else:
        result = "failed"
    print(name,"son of",fname,"has",result,"with total numbers", total_marks_obtained)
