# ESEP Grade Calculator

This library is a simple utility to calculate your grades.

Runtime requirements:
Golang 1.24+

## Usage
```go
gc := NewGradeCalculator()
gc.AddGrade("hw1", 95, Assignment)
gc.AddGrade("midterm", 88, Exam)
gc.AddGrade("essay 1", 92, Essay)
grade := gc.GetFinalGrade() 
```

Run unit tests:
```
cd grade_calculator/
go test ./...
```

Run unit tests with code coverage:
```
cd grade-calculator/
go test -coverprofile=coverage.txt ./...
go tool cover -func=coverage.txt
```