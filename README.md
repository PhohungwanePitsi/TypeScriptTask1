type Employee = {
  fullName: [string, string]; // Tuple: [firstName, lastName]
  age: number;
  department: string;
  skills: string[];
  isActive: boolean;
};


const employee1: Employee = {
  fullName: ["John", "Doe"],
  age: 30,
  department: "Engineering",
  skills: ["JavaScript", "Python", "C++"],
  isActive: true
};

const employee2: Employee = {
  fullName: ["Jane", "Smith"],
  age: 25,
  department: "Marketing",
  skills: ["SEO", "Social Media", "Content Creation"],
  isActive: false
};


function logEmployee(emp: Employee): void {
  console.log("--- Employee Details ---");
  console.log(`Name: ${emp.fullName[0]} ${emp.fullName[1]}`);
  console.log(`Age: ${emp.age}`);
  console.log(`Department: ${emp.department}`);
  console.log(`Skills: ${emp.skills.join(", ")}`);
  console.log(`Active: ${emp.isActive ? "Yes" : "No"}`);
  console.log("------------------------");
}


logEmployee(employee1);
logEmployee(employee2);
