# DevStack - Technology Stack Builder

A simple and interactive React web app where developers can browse different technologies and build their own custom tech stack for projects.

## 🔗 Links
- **Live Site:** https://comforting-kangaroo-581cec.netlify.app/
- **GitHub Repository:** https://github.com/iam-rajuahmmed/ph-assignment-5.git

## 🛠️ Technologies Used
- React.js (Vite)
- Tailwind CSS
- React-Toastify
- Lucide React

## ✨ Key Features
1. **Browse Technologies:** Explore various technologies categorized into Frontend, Backend, Database, and Tools.
2. **Build Custom Stack:** Add technologies to the stack list with a single click, with duplicate item prevention and toast alerts.
3. **Manage & Clear:** Remove individual items from the stack or clear the entire stack with one click.

---

## ❓ React Questions & Answers

### 1. What is JSX, and why is it used in React?
**Answer:** JSX stands for JavaScript XML. It allows us to write HTML-like code inside JavaScript. It makes writing and understanding component UI structure easier and cleaner.

### 2. What is the difference between props and state?
**Answer:**
- **Props:** Passed from parent to child component and are read-only (immutable).
- **State:** Managed internally within a component and can be changed over time (mutable), triggering a re-render when updated.

### 3. What does the `useState` hook do, and where did you use it in this project?
**Answer:** `useState` is a hook that allows functional components to create and update state variables. In this project, I used it for:
- Storing fetched technologies data (`technologies`)
- Managing the selected stack list (`selectedStack`)
- Handling loading state (`isLoading`)

### 4. What does the `useEffect` hook do, and why did you need it to load the JSON data?
**Answer:** `useEffect` handles side effects in React components (like data fetching). I used it with an empty dependency array `[]` to fetch the JSON data once when the component initially mounts, preventing infinite fetch loops.

### 5. Why does every item in a `.map()` list need a unique `key` prop?
**Answer:** The `key` prop helps React identify which items have changed, added, or removed. It optimizes performance during virtual DOM diffing so React only re-renders the specific updated items instead of the whole list.

### 6. What is conditional rendering? Show one place you used it.
**Answer:** Conditional rendering means rendering different UI elements based on certain conditions.
**Example:** In the sidebar, if the stack is empty (`stack.length === 0`), it shows an empty state message ("Your stack is empty"). When items exist, it renders the list of selected technologies.

### 7. How do you pass data from a parent component to a child component, and how does a child send something back to the parent?
**Answer:**
- **Parent to Child:** Data is passed down using **props** (e.g., `<Card tech={item} />`).
- **Child to Parent:** The parent passes a **callback function** as a prop, and the child calls that function with data when an event (like a button click) occurs. 

**------------------------------------------------------------------**
**NOTE: ALL Question Answer Answered By AI (ChatGPT) Assistant.**
**------------------------------------------------------------------**
