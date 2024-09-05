### Test Task for 2-Year Frontend Developer

#### **Objective**:
Create a full-stack web application using **Next.js (App Router)**, **Redux**, **Tailwind CSS**, **Node.js**, and **Express.js** that allows users to create, edit, delete, and upload files related to posts. Additionally, implement pagination, sorting, and unit testing using **Jest**.

---

### **Requirements**:

#### **Frontend**:
1. **Next.js (App Router)**:
    - Utilize the **App Router** feature in Next.js for routing and layouts.
    - Structure the app using **nested routes** and **shared layouts**.
    - Implement **server components** and **client components** effectively where needed.
    - Implement **SSR** (server-side rendering) or **SSG** (static site generation) for optimized performance:
        - The list of posts should be server-side rendered or statically generated.
        - Provide pagination and sorting options for the list of posts.
        - Handle form submissions using **Next.js API routes** for creating, editing, deleting posts, and uploading files.

2. **Pagination**:
    - Implement pagination to display posts in chunks (e.g., 10 posts per page).
    - Allow users to navigate between pages to view more posts.

3. **Sorting**:
    - Implement sorting functionality for posts (e.g., sort by date, title, or number of likes).
    - Sorting should be accessible via dropdown or table headers.

4. **File Upload**:
    - Allow users to upload files (e.g., images) when creating or editing a post.
    - Display uploaded files (e.g., image thumbnails) in the list of posts.
    - Implement the file upload feature on the frontend and handle file storage on the backend.

5. **Redux**:
    - Use **Redux** to manage global state for posts, pagination, sorting, and user authentication (basic login status).
    - Integrate Redux into the Next.js app using the **next-redux-wrapper** to handle server-side Redux state management.

6. **Tailwind CSS**:
    - Style the application using **Tailwind CSS**.
    - The main layout should include:
      - A header with the app’s title, sorting options, and user login status.
      - A form to create/edit posts with an option to upload files.
      - A paginated card or list layout to display the posts, with sorting functionality.

7. **Responsive Design**:
    - Ensure that the UI is fully responsive and works well across different screen sizes (mobile, tablet, and desktop).

#### **Backend**:
1. **Node.js & Express.js**:
    - Create a RESTful API using **Express.js** to manage the following:
      - `GET` /posts – fetch all posts with pagination and sorting.
      - `POST` /posts – create a new post, including file upload.
      - `PUT` /posts/:id – update an existing post, including file upload.
      - `DELETE` /posts/:id – delete a post.
    - Store posts in-memory (no database required for this task).
    - Implement a basic file storage solution (e.g., saving files locally) for handling file uploads.

2. **File Upload Handling**:
    - Use **Multer** or a similar middleware for handling file uploads in the Express.js backend.
    - Store uploaded files in a local directory and serve them via the backend.

3. **Integration with Next.js API Routes**:
    - Alternatively, handle file upload, pagination, and sorting logic using **Next.js API routes** directly, instead of Express.js.

#### **Unit Testing**:
1. **Jest**:
    - Write unit tests for key components such as the post list, pagination, and sorting functionality.
    - Write unit tests for Redux actions and reducers.
    - Write tests for API routes or backend services (if using Next.js API routes or Express.js).
    - Ensure file upload functionality is properly tested.

---

### **Additional Requirements**:
1. **Project Structure**:
    - Organize the project with a clear folder structure for components, API routes, Redux store, services, and file storage.

2. **Deployment**:
    - Deploy the application locally and provide instructions on how to run both the frontend and backend (if using Express.js).

3. **Documentation**:
    - Include a `README.md` with:
      - Instructions on setting up the environment.
      - Steps to run the app.
      - Instructions for running tests.
      - An overview of the project structure.
      - Instructions on how to upload files.

---

### **Evaluation Criteria**:
- **Correctness**: Does the app meet the functional requirements?
- **Code quality**: Is the code well-structured, clean, and follows best practices?
- **State management**: Effective use of Redux for managing the app’s state, including pagination, sorting, and file uploads.
- **UI/UX**: Does the UI look good, is it styled with Tailwind CSS, and is it responsive?
- **Testing**: Are there sufficient unit tests, and do they pass?
- **Performance**: Proper usage of Next.js App Router for server-side rendering and static generation.
- **File handling**: Is file upload, storage, and display working properly?
- **Pagination & Sorting**: Are the pagination and sorting features working as expected?

---

### **Bonus**:
- **Authentication**: Implement a basic login/logout mechanism using **NextAuth.js** or any preferred authentication method.
- **SEO**: Add basic SEO optimizations such as metadata and improved page titles.
- **Error Handling**: Implement proper error handling for file uploads and pagination/sorting requests.
