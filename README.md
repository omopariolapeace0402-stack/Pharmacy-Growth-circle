# Pharmacy-Growth-circle
Pharmacy student survival guide
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pharmacy Growth Circle: Seniors' Survival Guide</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&family=Playfair+Display:wght@700&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #f5f7fa 0%, #e4edf5 100%);
            padding: 30px;
        }
        
        .container {
            max-width: 1000px;
            margin: 0 auto;
            background: white;
            border-radius: 20px;
            box-shadow: 0 15px 40px rgba(0, 0, 0, 0.1);
            overflow: hidden;
        }
        
        .header {
            background: linear-gradient(135deg, #6a11cb 0%, #2575fc 100%);
            color: white;
            padding: 50px 40px;
            text-align: center;
            position: relative;
        }
        
        .header::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path fill="%23ffffff" fill-opacity="0.1" d="M0,224L48,213.3C96,203,192,181,288,181.3C384,181,480,203,576,192C672,181,768,139,864,138.7C960,139,1056,181,1152,186.7C1248,192,1344,160,1392,144L1440,128L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"></path></svg>');
            background-size: cover;
            background-position: bottom;
        }
        
        .header-content {
            position: relative;
            z-index: 1;
        }
        
        .header h1 {
            font-family: 'Playfair Display', serif;
            font-size: 2.8em;
            font-weight: 700;
            margin-bottom: 15px;
            text-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
        }
        
        .header .subtitle {
            font-size: 1.3em;
            font-weight: 300;
            opacity: 0.9;
            max-width: 700px;
            margin: 0 auto;
        }
        
        .content {
            padding: 50px 40px;
        }
        
        .section {
            margin-bottom: 50px;
        }
        
        .section-title {
            display: flex;
            align-items: center;
            margin-bottom: 25px;
            padding-bottom: 15px;
            border-bottom: 2px solid #eaeaea;
        }
        
        .section-icon {
            font-size: 1.8em;
            margin-right: 15px;
        }
        
        .section-title-text {
            font-family: 'Playfair Display', serif;
            font-size: 1.8em;
            font-weight: 700;
            color: #2c3e50;
        }
        
        .challenge-category {
            margin-bottom: 25px;
        }
        
        .category-title {
            font-weight: 600;
            color: #6a11cb;
            margin-bottom: 10px;
            font-size: 1.2em;
            display: flex;
            align-items: center;
        }
        
        .category-title::before {
            content: "•";
            margin-right: 10px;
            color: #6a11cb;
            font-size: 1.5em;
        }
        
        .challenge-list {
            list-style-type: none;
            padding-left: 20px;
        }
        
        .challenge-list li {
            margin-bottom: 10px;
            padding-left: 25px;
            position: relative;
        }
        
        .challenge-list li::before {
            content: "→";
            position: absolute;
            left: 0;
            color: #6a11cb;
            font-weight: bold;
        }
        
        .advice-category {
            background: #f8f9ff;
            border-radius: 12px;
            padding: 20px;
            margin-bottom: 25px;
            border-left: 4px solid #2575fc;
        }
        
        .advice-title {
            font-weight: 600;
            color: #2575fc;
            margin-bottom: 15px;
            font-size: 1.2em;
            display: flex;
            align-items: center;
        }
        
        .advice-title::before {
            content: "💡";
            margin-right: 10px;
        }
        
        .advice-list {
            list-style-type: none;
        }
        
        .advice-list li {
            margin-bottom: 10px;
            padding-left: 25px;
            position: relative;
        }
        
        .advice-list li::before {
            content: "✓";
            position: absolute;
            left: 0;
            color: #2575fc;
            font-weight: bold;
        }
        
        .wishes-table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            border-radius: 10px;
            overflow: hidden;
        }
        
        .wishes-table th {
            background: linear-gradient(135deg, #6a11cb 0%, #2575fc 100%);
            color: white;
            padding: 15px;
            text-align: left;
            font-weight: 600;
        }
        
        .wishes-table td {
            padding: 15px;
            border-bottom: 1px solid #eaeaea;
        }
        
        .wishes-table tr:nth-child(even) {
            background-color: #f8f9ff;
        }
        
        .wishes-table tr:hover {
            background-color: #eef2ff;
        }
        
        .category-cell {
            font-weight: 600;
            color: #2c3e50;
            width: 25%;
        }
        
        .footer {
            background: #2c3e50;
            color: white;
            text-align: center;
            padding: 30px 40px;
            font-size: 0.9em;
        }
        
        .footer p {
            margin-bottom: 10px;
        }
        
        .heart {
            color: #e74c3c;
        }
        
        @media (max-width: 768px) {
            body {
                padding: 15px;
            }
            
            .header {
                padding: 30px 20px;
            }
            
            .header h1 {
                font-size: 2.2em;
            }
            
            .content {
                padding: 30px 20px;
            }
            
            .section-title-text {
                font-size: 1.5em;
            }
            
            .wishes-table {
                display: block;
                overflow-x: auto;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <div class="header-content">
                <h1>Pharmacy Growth Circle: Seniors' Survival Guide</h1>
                <div class="subtitle">Your one-stop guide to surviving and thriving in the next level!</div>
            </div>
        </div>
        
        <div class="content">
            <div class="section">
                <div class="section-title">
                    <div class="section-icon">🔥</div>
                    <div class="section-title-text">Biggest Challenges Encountered During This Level</div>
                </div>
                <p style="margin-bottom: 25px; color: #555;">Here are the primary hurdles and difficulties faced by your seniors. Understanding these challenges can help you prepare mentally and practically.</p>
                
                <div class="challenge-category">
                    <div class="category-title">Academic Workload & Intensity</div>
                    <ul class="challenge-list">
                        <li>The bulkiness and sheer volume of the academic workload.</li>
                        <li>Heavy academic load and long school hours, which leave little personal time.</li>
                        <li>Understanding the PCG materials and practicals.</li>
                        <li>Difficulty with ANS Pharmacology.</li>
                    </ul>
                </div>
                
                <div class="challenge-category">
                    <div class="category-title">Time, Stress & Adjustment</div>
                    <ul class="challenge-list">
                        <li>Coping with stress and adapting to the abrupt changes in the curriculum.</li>
                        <li>Adjusting to the new level and mastering time management.</li>
                        <li>Trying to adapt to new things and balance all areas of life.</li>
                        <li>The challenge of balancing school, mental health, and personal life.</li>
                    </ul>
                </div>
                
                <div class="challenge-category">
                    <div class="category-title">Motivation & Consistency</div>
                    <ul class="challenge-list">
                        <li>Consistent lack of motivation and interest in studying.</li>
                        <li>Finding enough time to study.</li>
                    </ul>
                </div>
                
                <div class="challenge-category">
                    <div class="category-title">Specific Pain Points</div>
                    <ul class="challenge-list">
                        <li>Manual filing and practical sessions.</li>
                        <li>Inability to grab Oloton and Godfrey materials on time.</li>
                        <li>Exams and overall inconsistency.</li>
                    </ul>
                </div>
            </div>
            
            <div class="section">
                <div class="section-title">
                    <div class="section-icon">💡</div>
                    <div class="section-title-text">Essential Advice & Tips for Success</div>
                </div>
                <p style="margin-bottom: 25px; color: #555;">The seniors have spoken! Prioritize these action steps to ensure a smoother transition and academic success.</p>
                
                <div class="advice-category">
                    <div class="advice-title">Study Strategies</div>
                    <ul class="advice-list">
                        <li>Start early and be consistent—every little bit counts.</li>
                        <li>Read at every opportunity, even during short breaks.</li>
                        <li>Prioritize lecturer notes and take every aspect of the course seriously.</li>
                        <li>Get a suitable reading schedule on time.</li>
                        <li>Don't let practical workbook filling eat into your study time.</li>
                    </ul>
                </div>
                
                <div class="advice-category">
                    <div class="advice-title">Time & Focus</div>
                    <ul class="advice-list">
                        <li>Learn to manage time wisely; never procrastinate.</li>
                        <li>Don't wait till exams to start studying.</li>
                        <li>Don't miss classes, and cover material promptly.</li>
                    </ul>
                </div>
                
                <div class="advice-category">
                    <div class="advice-title">Mindset & Support</div>
                    <ul class="advice-list">
                        <li>Know your God and know yourself; this will help you scale through.</li>
                        <li>Be resilient, hardworking, and zealous.</li>
                        <li>Find your people on time; you will need a supportive circle.</li>
                        <li>Relate with helpful people and avoid stress.</li>
                        <li>Always find moments to de-stress—burnout is real.</li>
                        <li>Leverage the help of seniors.</li>
                    </ul>
                </div>
                
                <div class="advice-category">
                    <div class="advice-title">Course Specific Tip</div>
                    <ul class="advice-list">
                        <li>Know ANS Physiology well; it greatly helps in understanding ANS Pharmacology.</li>
                    </ul>
                </div>
            </div>
            
            <div class="section">
                <div class="section-title">
                    <div class="section-icon">✍️</div>
                    <div class="section-title-text">What Seniors Wish They Knew Earlier</div>
                </div>
                <p style="margin-bottom: 25px; color: #555;">These are the lessons learned in hindsight—insights that could have helped them plan and prepare better.</p>
                
                <table class="wishes-table">
                    <thead>
                        <tr>
                            <th>Category</th>
                            <th>Key Wish/Insight</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td class="category-cell">Mindset</td>
                            <td>It's okay to not have everything figured out. Don't compare yourself to others.</td>
                        </tr>
                        <tr>
                            <td class="category-cell">Preparation</td>
                            <td>Some courses aren't as hard as they seem; have the correct mindset.</td>
                        </tr>
                        <tr>
                            <td class="category-cell">Academic Reality</td>
                            <td>200 level will stretch you beyond your limit, but if you adapt, you can continue.</td>
                        </tr>
                        <tr>
                            <td class="category-cell">Pacing</td>
                            <td>Consistency matters more than speed. Find your balance early.</td>
                        </tr>
                        <tr>
                            <td class="category-cell">Specifics</td>
                            <td>Wish they were warned about PCG.</td>
                        </tr>
                        <tr>
                            <td class="category-cell">Study Habits</td>
                            <td>To print out materials instead of relying on soft copies.</td>
                        </tr>
                        <tr>
                            <td class="category-cell">Warning</td>
                            <td>It doesn't get easier. Put in the effort, and cover material promptly because more is coming.</td>
                        </tr>
                        <tr>
                            <td class="category-cell">Time Management</td>
                            <td>To manage time very well and never procrastinate.</td>
                        </tr>
                    </tbody>
                </table>
            </div>
        </div>
        
        <div class="footer">
            <p>Made with <span class="heart">💖</span> for Pharmacy Students</p>
            <p>Pharmacy Growth Circle © 2025</p>
        </div>
    </div>
</body>
</html>
