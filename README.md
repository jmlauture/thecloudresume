Thecloudresume </br>
•  🚀 About Me </br>
•  📌 Project overview  </br>
•  🧱 Architecture diagram </br>
•  🔧 Technologies used  </br>
•  🚀 Deployment steps </br>
•  🐛 Challenges & fixes </br>
•  💡 Engineering Philosophy </br>

🚀 About Me </br>
I combine a strong Database foundation with hands-on AWS cloud engineering experience to build scalable, secure, reliable, and cost-efficient solutions. I’m having fun building and deploying cloud applications using AWS. </br>

📌 Project overview </br>
The Cloud Resume Challenge goal is a multi-tier project requiring a serverless backend, a global CDN, and a fully automated CI/CD pipeline. The final product is a static resume website with visitor counts tracked and recorded in a DynamoDB table. </br>

🧱 Architecture diagram </br>
 
🔧 Technologies used </br>
•	Amazon Simple Storage Service (S3), AWS CLI </br>
•	Serverless Architecture (API Gateway, Lambda, DynamoDB) </br>
•	Amazon CloudFront (Content Delivery Network (CDN)) </br>
•	Amazon Route 53 (domain name pointing to CloudFront) </br>
•	Automation (Python, Shell scripting) </br>
•	Amazon CloudWatch (Monitoring) </br>
•	GitHub, GitHub actions (CI / CD) </br>

🚀 Deployment steps </br>
The full-stack serverless application is deployed on a platform with three layers. </br>
1. The Front-End (The "Static" Layer) </br>
•	S3 Bucket: Acts as the origin server where the HTML resume and eventual CSS files are stored. </br>
•	Amazon CloudFront: Acts as the Content Delivery Network (CDN) to serve the site over HTTPS. </br>
•	Amazon Route 53: Used to register / server a custom domain and point it to the CloudFront distribution. </br>

2. The Back-End (The "Logic" Layer) </br>
•	Amazon API Gateway: Provides a RESTful endpoint that the front-end (JavaScript) calls to retrieve or update data (like a visitor counter). </br>
•	AWS Lambda: A serverless function (written in Python) that handles the logic of reading from and writing to the database. </br>
•	Amazon DynamoDB: A NoSQL database that stores the visitor count. </br>

3. The DevOps Layer (Automation) </br>
•	GitHub Actions: The "CI/CD" engine. When I push or make changes in code on GitHub, an "Action" automatically updates the S3 bucket and invalidates the CloudFront cache.</br>

🐛 Challenges & fixes </br>
•	Fixed API Gateway "Not Found" errors caused by incorrect route configuration </br>
•	Resolved CORS issues blocking frontend API calls </br>
•	Debugged CloudFront caching delays after deployment </br>
•	Fixed Lambda permission issue to DynamoDB adhering to the principle of Least Privilege (Polp) </br>

💡 Engineering Philosophy </br>
Build → Measure → Optimize </br>
Cloud engineering is not just about deploying systems, but designing them for efficiency, scalability, and cost. </br>

🎯 Next Steps </br>
I plan to continue building on this project and explore more AWS features like: </br> 
•	Contact form → Lambda + SES </br>
•	Infrastructure as Code → CloudFormation </br>
•	Monitoring → CloudWatch dashboard </br>
•	… </br>
