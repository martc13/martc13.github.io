    <!DOCTYPE html>
    <html lang="en">
<!-- 
SA: I Charlise Martin, 400469676 certify that this material is my original work.
No other person's work has been used without due acknowledgement.
I have also not made my work available to anyone else.
-->
    <title> Charlise Martin 4IT3 Assignment #1 </title>

    <head>
    <style>
        body{
            font-family: 'Times New Roman', Times, serif;
            background: #f0f0f0;
            padding: 40px;
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            gap: 40px;
        }

        .main-content{
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 30px;
        }

        .container{
            display: flex;
            gap: 40px; 
            max-width: 1500px; 
            width: 100%;
            justify-content: center;
            flex-wrap: nowrap;
            align-items: flex-start;
        }

        .bubble-content{
            flex: 1;
            display: flex;
            flex-direction: column;
            gap: 25px;
            position:sticky;
            top:40px; 
            align-items: center;
            justify-content: flex-start;
        }

        .bubble{
            width: 180px;
            height: 180px;
            border-radius: 50%;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding: 20px;
            color: black;
            font-weight: bold;
            font-size: 18px;
            box-shadow: 0 8px 15px rgba(0, 0, 0, 0.203);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            cursor: default;
            position: relative;
            background:linear-gradient(135deg,rgb(196, 240, 247),rgb(247, 200, 248));
            animation: float 3s ease-in-out infinite alternate;
        }

        .bubble:hover{
            transform: scale(1.05) rotate(-1deg);
            box-shadow: 0 12px 20px rgba(0,0,0,.2);
        }        

        .bubble b{
            display:block;
            margin-bottom: 8px;
            font-size: 20px;
        }

        .bubble p{
            font-weight: normal;
            font-size: 16px;
            margin: 0;
        }

        @keyframes float{
            0% { transform: translateY(0px) rotate(0deg); }
            50% { transform: translateY(-8px) rotate(2deg); }
            100% { transform: translateY(0px) rotate(-2deg); }
        }

        .bubble::before{
            content:'';
            position:absolute;
            top:-5px;
            left:-5px;
            width:calc(100% + 10px);
            height:calc(100% + 10px);
            border-radius:50%;
            filter: blur(12px);
            z-index:-1;
        }

        .badge{
            display:flex;
            flex-direction: column;
            align-items:center;
            gap:15px;
            background:linear-gradient(135deg,rgb(247, 200, 248),rgb(196, 240, 247));
            padding:15px 20px;
            border-radius:20px;
            width:500px;
            margin:0 auto;
            justify-content:center;
            text-align: center;
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.203);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .badge:hover{
            transform: scale(1.05) rotate(-1deg);
            box-shadow: 0 12px 20px rgba(0,0,0,.2);
        }

        .badge img{
            width:100px;
            height:100px;
            border-radius:100px;
            object-fit:cover;
            border:4px solid white;
        }

        .badge h1{
            margin:0;
            color: black;
            font-family: 'Times New Roman', Times, serif;
        } 

        .badge .contact-info{
            margin: 0;
            color: black;
            text-align: center;
        }

        .badge .contact-info a{
            color:black;
            text-decoration: none;
        }

        .badge .contact-info a:hover{
            text-decoration: underline;
        }

        .display{
            display:flex;
            gap:20px;
            justify-content:center;
            flex-wrap: wrap;
        }

        .box{
            background:linear-gradient(135deg,rgb(247, 200, 248),rgb(196, 240, 247));
            padding:12px 16px;
            border-radius:14px;
            font-family: 'Times New Roman', Times, serif;
            width:220px;
            text-align: center;
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.203);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

         .box:hover{
            transform: scale(1.05) rotate(-1deg);
            box-shadow: 0 12px 20px rgba(0,0,0,.2);
        }

        .box h3{
            margin-bottom: 6px;
        }

        .box p{
            margin:0;
        }

        .title{
            text-align: center;
            font-family: 'Times New Roman', Times, serif;
            font-size: 32px;
            color: black;
            position:relative;
            margin-bottom: 20px;
        }

        .title::after{
            content:'';
            display:block;
            width:120px;
            height:6px;
            background: linear-gradient(135deg,rgb(246, 159, 249),rgb(138, 228, 242));
            margin:10px auto 0 auto;
            border-radius: 3px;
        }

        .job-link{
            color: black;
            text-decoration: none;
        }

        .job-link:hover{
            text-decoration: underline;
        }

    </style>
    </head>

    <body> 
    <div class = "container">
        <div class="bubble-content">
            <div class="bubble"> 
                <b>Technical Skills</b>
                <p>Programming, Laboratory Experience, Chemical Engineering</p>
            </div>

            <div class="bubble"> 
                <b>Strengths</b>
                <p>Problem Solving, Teamwork, Communication, Time Management</p>
            </div>
            

            <div class="bubble"> 
                <b>Awards</b>
                <p>Honor Roll Student, Ontario Scholar Award, Student Union Award</p>
            </div>

        </div>
        <div class="main-content">
            <section>
                <div class="badge">
                    <img src="Charlise_Professional_Image.jpg" alt="Charlise Martin">
                    <h1>Charlise Martin</h1>
                    <p class="contact-info">martc13@mcmaster.ca</p>
                    <p class="contact-info">
                        <a href = "https://www.linkedin.com/in/charlise-martin/"> LinkedIn Profile </a>
                    </p>
                </div>
            </section>

            <section>
            <h2 class="title"> My Education </h2>
                <div class="display">
                    <div class="box"> 
                        <h3>McMaster University</h3>
                        <p>Automation Systems Engineering Technology</p>
                    </div>
                    <div class="box">
                        <h3>Westside Secondary School</h3>
                        <p>Orangeville, ON</p>
                    </div>
                </div>
            </section>

            <section>
                <h2 class="title"> My Work Experience </h2>
                <div class="display">
                    <div class="box"> 
                        <h3>Cashier at Walmart Canada</h3>
                        <p>(July 2021 - August 2022)</p>
                    </div>
                    <div class="box">
                        <h3>Lot attendant at MacMaster Buick GMC</h3>
                        <p>(May 2023 - June 2024)</p>
                    </div>
                    <div class="box">
                        <h3>LES Project Assistant Co-op at Thermo Fisher Scientific</h3>
                        <p>(June 2024 - August 2025)</p>
                    </div>
            </section>
            <section>
                <div class="display">
                    <div class="box"> 
                        <p>Cashed out and served with more than 100 customers on a day-to-day basis to assist with any needs or concerns</p>
                        <hr>
                        <p>Cleaned and maintained the till in between customers to keep till looking more appealing for customers</p>
                        <hr>
                        <p>Worked and communicated in a team setting with 6 to 10 people throughout the day to better support customers</p>
                    </div>
                    <div class="box">
                        <p>Worked and communicated with two managers and a team of 3 people to ensure the cars on the lot were presented to customers as effectively as possible</p>
                        <hr>
                        <p>Ensured all of the price tags were hung in the rear view mirror of all vehicles</p>
                        <hr>
                        <p>Drove vehicles to and from the professional cleaners, mechanics and customers</p>
                    </div>
                    <div class="box">
                        <p>Develop new lab methods as digital workflows in the SM-LES system, using paper-based lab methods as a template.</p>
                        <hr>
                        <p>Assist with the implementation of basic instruments and calibrations through the SM-LES system. </p>
                        <hr>
                        <p>Support the LIMS project by updating the electronic sample database for both analytical and microbiological labs, including tasks like stability studies, sample tracking, logging, and method workflows.</p>
                    </div>
                </div>
            </section>
            <section>
            <div class="display">
                <div class="box"> 
                    <a href = "https://www.walmart.ca/en" class="job-link"> Walmart Canada Website </a>
                </div>
                <div class="box">
                    <a href = "https://www.macmastergm.com/" class="job-link"> MacMaster Buick GMC Website </a> <br/><br/>
                </div>
                <div class="box">
                    <a href = "https://www.thermofisher.com/ca/en/home.html" class="job-link"> Thermo Fisher Website </a> <br/><br/> 
                </div>
            </div>
        </section>
        </div>
        
        <div class="bubble-content">
            <div class="bubble"> 
                <b>Hobbies</b>
                <p>Painting & Gardening</p>
            </div>

            <div class="bubble"> 
                <b>Favourite Sit-Coms</b>
                <p>New Girl, Superstore, Brooklyn 99</p>
            </div>

            <div class="bubble"> 
                <b>Professional Association</b>
                <p>BTA Social Media Coordinator</p>
            </div>
        </div>  
    </div>  
    
</body>
</html>
