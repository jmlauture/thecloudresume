Thecloudresume
•  🚀 About Me
•  📌 Project overview 
•  🧱 Architecture diagram 
•  🔧 Technologies used  
•  🚀 Deployment steps 
•  🐛 Challenges & fixes 
•  💡 Engineering Philosophy


🚀 About Me
I combine a strong Database foundation with hands-on AWS cloud engineering experience to build scalable, secure, reliable, and cost-efficient solutions. I’m having fun building and deploying cloud applications using AWS.
📌 Project overview
The Cloud Resume Challenge goal is a multi-tier project requiring a serverless backend, a global CDN, and a fully automated CI/CD pipeline. The final product is a static resume website with visitor counts tracked and recorded in a DynamoDB table.

🧱 Architecture diagram
 
🔧 Technologies used
•	Amazon Simple Storage Service (S3), AWS CLI 
•	Serverless Architecture (API Gateway, Lambda, DynamoDB)
•	Amazon CloudFront (Content Delivery Network (CDN))
•	Amazon Route 53 (domain name pointing to CloudFront)
•	Automation (Python, Shell scripting)
•	Amazon CloudWatch (Monitoring)
•	GitHub, GitHub actions (CI / CD)

🚀 Deployment steps 
The full-stack serverless application is deployed on a platform with three layers.
1. The Front-End (The "Static" Layer)
•	S3 Bucket: Acts as the origin server where the HTML resume and eventual CSS files are stored.
•	Amazon CloudFront: Acts as the Content Delivery Network (CDN) to serve the site over HTTPS.
•	Amazon Route 53: Used to register / server a custom domain and point it to the CloudFront distribution.
2. The Back-End (The "Logic" Layer)
•	Amazon API Gateway: Provides a RESTful endpoint that the front-end (JavaScript) calls to retrieve or update data (like a visitor counter).
•	AWS Lambda: A serverless function (written in Python) that handles the logic of reading from and writing to the database.
•	Amazon DynamoDB: A NoSQL database that stores the visitor count.
3. The DevOps Layer (Automation)
•	GitHub Actions: The "CI/CD" engine. When I push or make changes in code on GitHub, an "Action" automatically updates the S3 bucket and invalidates the CloudFront cache.
🐛 Challenges & fixes 
•	Fixed API Gateway "Not Found" errors caused by incorrect route configuration
•	Resolved CORS issues blocking frontend API calls
•	Debugged CloudFront caching delays after deployment
•	Fixed Lambda permission issue to DynamoDB adhering to the principle of Least Privilege (Polp)
💡 Engineering Philosophy
Build → Measure → Optimize
Cloud engineering is not just about deploying systems, but designing them for efficiency, scalability, and cost.

🚀 Next Steps 
I plan to continue building on this project and explore more AWS features like: 
•	Contact form → Lambda + SES
•	Infrastructure as Code → CloudFormation 
•	Monitoring → CloudWatch dashboard
•	…


🎯 Career Objective <br/>
Seeking opportunities as a Cloud Database Engineer / Cloud Engineer where I can contribute to scalable and reliable systems.
