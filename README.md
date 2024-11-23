# PELEC201_FALNICAN
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Student Enrollment Form</title>
    <link rel="stylesheet" href="style.css"> <!-- Link to external CSS -->
</head>
<body>
    <div class="wrapper">
        <!-- Header -->
        <h1>Student Registration Form</h1>

        <!-- Instructions -->
        <h2>Welcome to Dalubhasaan ng Lungsod ng Lucena</h2>
        <ol>
            <li>To enroll you must fill in the form.</li>
            <li>Now, you need to select what course and what field you're interested.</li>
            <li>For the final step, you need to click "Enroll Now" to submit.</li>
        </ol>

        <!-- Enrollment Form -->
        <form action="/submit" method="POST">
            <!-- Full Name -->
            <label for="fullName"id='form-text'>Full Name:</label>
            <input type="text" id="fullName" name="fullName" placeholder="Enter your name" required>

            <!-- Email -->
            <label for="email" id="form-text">Email Address:</label>
            <input type="email" id="email" name="email" placeholder="Enter your email" required>

            <!-- Age -->
            <label for="age" id="form-text">Age:</label>
            <input type="number" id="age" name="age" placeholder="Enter your age" required>

            <!-- Sex -->
            <label id="form-text">Sex:</label>
            
            <label for="male" id="male">Male</label>
            <input type="radio" id="male" name="sex" value="Male" required>
            
            <label for="female" id="female">Female</label>
            <input type="radio" id="female" name="sex" value="Female" required>

            <!-- Course Options -->
            <label for="course" id="form-text">Course:</label>
            <select id="course" name="course" required>
                <option value="">Select a course</option>
                <option value="BSIT">BSIT</option>
                <option value="BSA">BSA</option>
                <option value="BSSW">BSSW</option>
                <option value="BSPA">BSPA</option>
                <option value="DHRS">DHRS</option>
                <option value="BSAIS">BSAIS</option>
            </select>

            <!-- Interests -->
            <label id="form-text">For Information Technology, choose in what field you're interested:</label>
            <div id="interest">
                <input type="checkbox" id="webDev" name="interests" value="Web Development">
                <label for="web_dev" id="web_dev">Web Development</label>
                <br>
                <input type="checkbox" id="dataScience" name="interests" value="Data Science">
                <label for="data_science" id="data_science">Data Science</label>
                <br>
                <input type="checkbox" id="networking" name="interests" value="Networking">
                <label for="networking" id="networking">Networking</label>
                <br>
                <input type="checkbox" id="graphicDesign" name="interests" value="Graphic Design">
                <label for="graphic_design" id="graphic_design">Graphic Design</label>
            </div>


            <!-- Submit Button -->
            <button type="submit" id="enroll">Enroll Now</button>
        </form>

        <!-- Student Data Table -->
        <h3>Student Data</h3>
        <table>
            <thead>
                <tr>
                    <th>ID</th>
                    <th>Name</th>
                    <th>Email</th>
                    <th>Age</th>
                    <th>Sex</th>
                    <th>Course</th>
                    <th>Interests</th>
                </tr>
            </thead>
            <tbody>
                <!-- Dummy Student Data -->
                <tr>
                    <td>1</td>
                    <td>Agatha Harkness</td>
                    <td>agathaallalong@gmail.com</td>
                    <td>19</td>
                    <td>Female</td>
                    <td>BSIT</td>
                    <td>Web Development, Graphic Design</td>
                </tr>
                <tr>
                    <td>2</td>
                    <td>Rio Vidal</td>
                    <td>riovidal@gmail.com</td>
                    <td>20</td>
                    <td>Female</td>
                    <td>BSIT</td>
                    <td>Networking, Data Algorithm</td>
                </tr>
                    <td>3</td>
                    <td>Denise Julia</td>
                    <td>denisejulia@gmail.com/td>
                    <td>19</td>
                    <td>Female</td>
                    <td>BSIT</td>
                    <td>Graphic Design, Networking</td>
                <tr>
                    <td>4</td>
                    <td>Wanda Maximoff</td>
                    <td>wandamaximoff@gmail.com</td>
                    <td>19</td>
                    <td>Female</td>
                    <td>BSIT</td>
                    <td>Data Science, Graphic Design</td>
                </tr>
                <tr>
                    <td>5</td>
                    <td>Billy Kaplan</td>
                    <td>billy.kaplan@gmail.com</td>
                    <td>19</td>
                    <td>Male</td>
                    <td>BSIT</td>
                    <td>Web Development, Data Science</td>
                </tr>
            </tbody>
        </table>
    </div>
</body>
</html>

#CSS
[Uploading style.css…]()

/* General body styling */
body {
    font-family: "Arial", sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    background-image: url('DLL.jpg');
}
   
    /* Center the content */
.wrapper {
    width: 900px;
    background: rgba(7, 50, 88, 0.486);
    border: 2px solid rgba(255, 255, 255, .2);
    box-shadow: 0 0px 10px rgba(0, 0, 0, .2);
    backdrop-filter: blur(50px);
    border-radius: 10px;
    color: #fff;
    padding: 40px 70px 40px;
}

/* Header styling */
.wrapper h1 {
    text-align: center;
    background-image: linear-gradient(43deg, #ffffff 0%, #348ec6 100%);
    background-clip: text;
    color: transparent;
    font-size: 3rem;![DLL](https://github.com/user-attachments/assets/206d58e3-cacf-43ce-99ff-4c89d18aead0)

    padding-bottom: 3rem;
}

/* Instructions styling */
.wrapper h3 {
    justify-content: center;
    text-align: center;
    color: rgb(255, 255, 255);
    margin-bottom: 10px;
    font-size: 1.8rem;
}

.wrapper ol li{
    margin: 0 0 20px 20px;
    color: rgb(255, 255, 255);
    font-size: 18px;
    
}

/* Form inputs */
.wrapper label {
    display: block;
    margin: 10px 0 5px;
    font-weight: bold;
}

.wrapper input, select, button, table {
    font-size: 14px;
}

.wrapper input, select {
    width: 100%;
    padding: 8px;
    margin-bottom: 10px;
    border: 1px solid #ccc;
    border-radius: 5px;
    box-sizing: border-box;
}

/* Checkbox and radio button styling */
.wrapper input[type="radio"], input[type="checkbox"] {
    width: auto;
    margin-right: 5px;
}

/* Submit button */
.wrapper button {
    width: 100%;
    padding: 10px;
    background-color: #0860a4;
    color: white;
    border: none;
    border-radius: 10px;
    cursor: pointer;
    margin-top: 30px;
    margin-bottom: 30px;
}

.wrapper button:hover {
    background-color: #1b3c6e;
}

/* Table styling */

.wrapper #form-text{
    padding-top: 10px;
    margin-top: 10px;
}

.wrapper table {
    width: 100%;
    border-collapse: collapse;
    margin-top: 20px;
}

.wrapper table th, table td {
    border: 1px solid #ddd;
    padding: 8px;
    text-align: center;
}

.wrapper table th {
    background-color: #345e8f;
    font-weight: bold;
}

.wrapper table tr:nth-child(even) {
    background-color: #164973;

}

.wrapper table tr:hover {
    background-color: #0965a2;
}

#web_dev{
    display: inline;
    margin-bottom: 20px;
    margin-top: 20px;
}
#data_science{
    display: inline;
    margin-bottom: 20px;
}
#networking{
    display: inline;
    margin-bottom: 10px;
}
#graphic_design{
    display: inline;
    margin-bottom: 50px;
}

#radio{
    padding-right: 20%;
}
.wrapper #male{
    display: inline;

}
.wrapper #female{
    display: inline;
}
