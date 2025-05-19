# Advanced HTML5 Elements and Forms

## Objectives
Implement HTML5 images, lists, tables, forms and input types.
Use form validation attributes.
Apply multimedia elements such as audio and video.

## Instructions

- Create an index.html file.
- Add an ordered list with roman numerals
- Add an external image from pexels.com
- Add a table of 5 contacts with; name, address, mobile and emails
- Add a registration form

>[!NOTE]
>  The registration form should have:
>- Name, email, password, and date fields.
>- A dropdown, radio buttons, and checkboxes.
>- Proper labels and placeholders.
>- Required fields and validation attributes.
>- Ensure proper indentation and commenting.
 
# Tasks
- Create a well-structured HTML5 document.
- Ensure semantic correctness.

Happy Coding! 💻✨
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML5 Features Demonstration</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        section {
            margin-bottom: 30px;
            padding: 20px;
            border: 1px solid #ddd;
            border-radius: 5px;
        }
        table {
            width: 100%;
            border-collapse: collapse;
        }
        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: left;
        }
        th {
            background-color: #f2f2f2;
        }
        form {
            display: grid;
            grid-gap: 15px;
        }
        label {
            font-weight: bold;
        }
        input, select, textarea {
            width: 100%;
            padding: 8px;
            box-sizing: border-box;
        }
        button {
            background-color: #4CAF50;
            color: white;
            padding: 10px 15px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <header>
        <h1>HTML5 Features Demonstration</h1>
    </header>

    <!-- Ordered List with Roman Numerals -->
    <section id="ordered-list">
        <h2>Top 5 Programming Languages (Ordered List with Roman Numerals)</h2>
        <ol type="I">
            <li>JavaScript</li>
            <li>Python</li>
            <li>Java</li>
            <li>C#</li>
            <li>PHP</li>
        </ol>
    </section>

    <!-- External Image from Pexels -->
    <section id="external-image">
        <h2>Beautiful Nature Image (from Pexels.com)</h2>
        <figure>
            <img src="https://images.pexels.com/photos/15286/pexels-photo.jpg" 
                 alt="Scenic mountain landscape with trees and fog" 
                 width="800"
                 height="500">
            <figcaption>Beautiful mountain landscape photo from Pexels</figcaption>
        </figure>
    </section>

    <!-- Contacts Table -->
    <section id="contacts-table">
        <h2>Contact List (Table)</h2>
        <table>
            <thead>
                <tr>
                    <th>Name</th>
                    <th>Address</th>
                    <th>Mobile</th>
                    <th>Email</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>John Smith</td>
                    <td>123 Main St, Anytown</td>
                    <td>555-0101</td>
                    <td>john.smith@example.com</td>
                </tr>
                <tr>
                    <td>Sarah Johnson</td>
                    <td>456 Oak Ave, Somewhere</td>
                    <td>555-0102</td>
                    <td>sarah.j@example.com</td>
                </tr>
                <tr>
                    <td>Michael Brown</td>
                    <td>789 Pine Rd, Nowhere</td>
                    <td>555-0103</td>
                    <td>m.brown@example.com</td>
                </tr>
                <tr>
                    <td>Emily Davis</td>
                    <td>321 Elm Blvd, Anywhere</td>
                    <td>555-0104</td>
                    <td>emily.d@example.com</td>
                </tr>
                <tr>
                    <td>David Wilson</td>
                    <td>654 Maple Ln, Everywhere</td>
                    <td>555-0105</td>
                    <td>dwilson@example.com</td>
                </tr>
            </tbody>
        </table>
    </section>

    <!-- Registration Form -->
    <section id="registration-form">
        <h2>Registration Form</h2>
        <form id="register" action="#" method="post">
            <!-- Name Field -->
            <div>
                <label for="name">Full Name*:</label>
                <input type="text" id="name" name="name" 
                       placeholder="Enter your full name" 
                       required 
                       minlength="3"
                       maxlength="50">
            </div>

            <!-- Email Field -->
            <div>
                <label for="email">Email*:</label>
                <input type="email" id="email" name="email" 
                       placeholder="Enter your email address" 
                       required>
            </div>

            <!-- Password Field -->
            <div>
                <label for="password">Password*:</label>
                <input type="password" id="password" name="password" 
                       placeholder="Create a password (min 8 characters)" 
                       required 
                       minlength="8"
                       pattern="^(?=.*[A-Za-z])(?=.*\d)[A-Za-z\d]{8,}$"
                       title="Must contain at least one letter and one number">
            </div>

            <!-- Date Field -->
            <div>
                <label for="birthdate">Date of Birth*:</label>
                <input type="date" id="birthdate" name="birthdate" 
                       required>
            </div>

            <!-- Dropdown Menu -->
            <div>
                <label for="country">Country:</label>
                <select id="country" name="country">
                    <option value="">Select your country</option>
                    <option value="us">United States</option>
                    <option value="ca">Canada</option>
                    <option value="uk">United Kingdom</option>
                    <option value="au">Australia</option>
                    <option value="other">Other</option>
                </select>
            </div>

            <!-- Radio Buttons -->
            <div>
                <label>Subscription Plan:</label>
                <div>
                    <input type="radio" id="free" name="plan" value="free" checked>
                    <label for="free">Free</label>
                </div>
                <div>
                    <input type="radio" id="premium" name="plan" value="premium">
                    <label for="premium">Premium ($9.99/month)</label>
                </div>
                <div>
                    <input type="radio" id="enterprise" name="plan" value="enterprise">
                    <label for="enterprise">Enterprise ($29.99/month)</label>
                </div>
            </div>

            <!-- Checkboxes -->
            <div>
                <label>Interests (select all that apply):</label>
                <div>
                    <input type="checkbox" id="tech" name="interests" value="tech">
                    <label for="tech">Technology</label>
                </div>
                <div>
                    <input type="checkbox" id="sports" name="interests" value="sports">
                    <label for="sports">Sports</label>
                </div>
                <div>
                    <input type="checkbox" id="music" name="interests" value="music">
                    <label for="music">Music</label>
                </div>
                <div>
                    <input type="checkbox" id="travel" name="interests" value="travel">
                    <label for="travel">Travel</label>
                </div>
            </div>

            <!-- Textarea -->
            <div>
                <label for="comments">Additional Comments:</label>
                <textarea id="comments" name="comments" 
                          placeholder="Any additional information..." 
                          rows="4"></textarea>
            </div>

            <!-- Submit Button -->
            <button type="submit">Register</button>
        </form>
    </section>

    <!-- Multimedia Elements -->
    <section id="multimedia">
        <h2>Multimedia Elements</h2>
        
        <!-- Audio -->
        <div>
            <h3>Audio Example</h3>
            <audio controls>
                <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
                Your browser does not support the audio element.
            </audio>
        </div>

        <!-- Video -->
        <div>
            <h3>Video Example</h3>
            <video width="800" height="450" controls>
                <source src="https://samplelib.com/lib/preview/mp4/sample-5s.mp4" type="video/mp4">
                Your browser does not support the video tag.
            </video>
        </div>
    </section>

    <footer>
        <p>&copy; 2023 HTML5 Features Demonstration. All rights reserved.</p>
    </footer>
</body>
</html>
