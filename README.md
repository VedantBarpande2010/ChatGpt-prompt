Objective:
The goal of this is to create a ChatGPT prompt that takes a resume as input and outputs the parsed content in JSON format. 

Prompt:
"You are given a resume in plain text format. Your task is to parse the content and convert it into JSON format. The JSON should contain the following keys: 'name', 'contact', 'summary', 'experience', 'education', 'skills', and 'certifications'. Each section should be appropriately extracted and formatted.

   Example resume:
   ```
   Yash Kumar
   123 Kothrud Pune
   (+91) 9656789282
   yashkumar@email.com

   Summary:
   Experienced software developer with expertise in web development and database management.

   Experience:
   Software Developer at TechCorp (Jan 2024 - Present)
   - Developed and maintained web applications.
   - Collaborated with cross-functional teams.

   Education:
   B-Tech in Mechanical Engineering , Savitribai University (2020 - 2024)

   Skills:
   - JavaScript
   - Python
   - SQL

   Certifications:
   - Complete Data analsyt Bootcamp by UDEMY

   JSON output:
   ```json
   {
     "name": " Yash Kumar",
     "contact": "123 Kothrud Pune , (+91) 9656789282 , yashkumar@email.com",
     "summary": "Experienced software developer with expertise in web development and database management.",
     "experience": [
       {
         "title": "Software Developer",
         "company": "TechCorp",
         "duration": "Jan 2024 - Present",
         "responsibilities": [
           "Developed and maintained web applications.",
           "Collaborated with cross-functional teams."
         ]
       }
     ],
     "education": [
       {
         "B-Tech in Mechanical Engineering , Savitribai University (2020 - 2024)"
       }
     ],
     "skills": [
       "JavaScript",
       "Python",
       "SQL"
     ],
     "certifications": [
       "Complete Data analsyt Bootcamp by UDEMY"
     ]
   }
   ```"

