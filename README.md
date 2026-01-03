if __name__ == '__main__':
    students =[]
    s = []
    for _ in range(int(input())):
        name = input()
        score = float(input())
        
        students.append([name, score])
        s.append(score)
        
   
    s = set(s)
    m = min(s)
    s.remove(m)
    s = min(s)
    students = sorted(students)  
    for x in range(len(students)):
        if students[x][1] == s:
            print(students[x][0])
