## How to setup tailwind css
 1. Run the following commands 

 npm install -d tailwindcss 
 npx tailwindcss init 

 step 2. update tailwind.conf.jsfile to include this line :

 ``` 
 content:["./*.html"]

 if your code is inside the src then write this 
content: ["./src/**/*.html"]

 step 3: create src/input.css to include : 
@tailwind base;
@tailwind components;
@tailwind utilities;

 step 4: Include the src/output.css file to your html 

 step 5. Run the following command :

 npx tailwindcss -i ./src/input.css -o ./src/output.css --watch

 we can also do this 
 To go to the package.json and in the script create a "build:css":"tailwindcss -i ./src/input.css -o ./src/output.css --watch"

 Then in the terminal write npm run build:css 
 every time when you open your vscode to change the directory in which you are working and now write" npm run build:css" in the terminal , then you will watch that your code is working perfectly .