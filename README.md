1. What was the most challenging part of building this API?
The most challenging part was connecting the API to the database and making sure everything worked correctly.

2. How does TypeORM make database operations easier compared to raw SQL?
TypeORM makes it easier because I can manage database records using JavaScript or TypeScript instead of writing SQL queries manually.

3. Why is it important to exclude the password field from API responses? How did you implement this?
It protects users' personal information and keeps their passwords private. I implemented this by excluding the password field when returning user data.

4. Describe a scenario where you would need to use database transactions instead of individual operations.
When transferring money between two accounts, a transaction ensures that both operations succeed. If one fails, both are cancelled.

5. What is the difference between synchronize: true and migrations? When should you use each?
synchronize: true automatically updates the database structure. Migrations require manual steps to update it. Synchronize is useful for practice, while migrations are better for production.

6. If you had to add a Product entity with a relationship to User (a user can have many products), how would you modify the code?
I would create a Product entity and use a ManyToOne relationship in Product and a OneToMany relationship in User.

7. What security improvements would you make before deploying this API to production?
I would add password hashing, authentication, rate limiting, input validation, and proper error handling to make the API more secure.