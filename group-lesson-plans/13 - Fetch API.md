## **Lesson 13: Fetch API & Async/Await — Group Mentor Guide**

Welcome to Lesson 13! This week, students transition from local data management to interacting with external servers using the **Fetch API**. They will learn to handle real-world data by pulling their own GitHub repositories into their portfolio and starting a new **Open API Project**.

### **Warm-Up (5–10 minutes)**
**Mindset: Problem Solving**
*   Share a time you faced a coding problem where you had "no idea how to get started." What was the first small step you took to chip away at it?
*   The sources mention a process: **understanding the problem, planning, and dividing it into subproblems**. Which of these three steps do you find the most difficult, and why?

### **Check for Understanding (Asynchronous Theory)**
*   What does the `fetch` function return? (Answer: A **Promise** that fulfills when the server response arrives).
*   How do the `async` and `await` keywords change how we write asynchronous code? (Answer: `async` ensures a function returns a promise; `await` pauses execution until a promise is resolved, making async code look and behave more like synchronous code).
*   What is the default HTTP method used by `fetch` if no options are provided? (Answer: **GET**).

### **Explore vs. Apply — Session Formats**
*   **Explore Sessions** → Walk through the structure of a `fetch` request, focusing on the two-step process of getting a response and then parsing it with `.json()`.
*   **Apply Sessions** → Live-code a simple fetch request to a public API (like JSONPlaceholder) or help students troubleshoot their GitHub repository loop.

###### **Sample Timing for 1-Hour Session**
| Time | Activity |
| :--- | :--- |
| 0:00–0:10 | Warm-up + Reviewing "Problem Solving" mindset |
| 0:10–0:25 | Explore: `fetch()` parameters (URL vs. options) and `async/await` syntax |
| 0:25–0:50 | Apply: Troubleshooting the GitHub API loop and dynamic `li` creation |
| 0:50–1:00 | Wrap-up: Checking the Open API project repository setup |

### **Check for Understanding (Ask 2–3)**
*   What is the purpose of checking `response.ok` before parsing the data? (Answer: To ensure the request was successful before trying to use the data).
*   Why is it important to use a `try...catch` block with `async/await`? (Answer: To handle potential errors from the server so the application doesn't crash).
*   How do you find the specific name of a repository from the array of objects returned by the GitHub API? (Answer: By accessing the `.name` property of each repository object during the loop).

### **Apply Prompts**
*   **Git Workflow:** Ensure students merge their `lesson-12` PR and pull to `main` before creating the `lesson-13` branch.
*   **Repository Hygiene:** Remind students **not** to clone their new Open API repository inside their portfolio folder, as this creates a "sub-repository" conflict.
*   **Looping Logic:** If students can see the data in the console but not the page, check if they are correctly using `appendChild` to add their new `li` elements to the `projectList`.
*   **README Links:** Remind students to add a link to their new Open API project in their portfolio's `readme.md` so reviewers can find it.
