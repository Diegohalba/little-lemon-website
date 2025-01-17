# Restaurant Table Booking System

A table-booking system using React. It's a fully responsive web app that allows users to reserve a table for the Little Lemon restaurant. 

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)

## Overview

### Screenshot

![restaurantBookingSystem](https://user-images.githubusercontent.com/111131083/404332236-bf7cd04b-4c03-4d0a-98c7-0235e2ea8c9f.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzcxMjM5NDcsIm5iZiI6MTczNzEyMzY0NywicGF0aCI6Ii8xMTExMzEwODMvNDA0MzMyMjM2LWJmN2NkMDRiLTRjMDMtNGQwYS05OGM3LTAyMzVlMmVhOGM5Zi5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwMTE3JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDExN1QxNDIwNDdaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1jYzc4OGJkMWExZWZkYjc5YWU5OWM2NTQ4N2Q1NDdjNjE2YTIzYWZkMzY2NmY0YTY3OWJmM2RiZDE5OTJmMjhiJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.me8gs_fRNF3alYAfluejCwpYBbU1mychWEH4RqEnunA)
![restaurantBookingSystem](src\assets\make-reservation.png)
![restaurantBookingSystem](src\assets\reservation-confirmed.png)


### Links

- Live : [Demo](https://little-lemon-website-eight.vercel.app/)

## My process

### Built with

- [React](https://beta.reactjs.org/) - React 
- [React Router v6+](https://reactrouter.com/en/main) - For routes
- [React Scroll](https://www.npmjs.com/package/react-scroll) - For smooth scroll
- [React Testing Library](https://testing-library.com/docs/react-testing-library/intro/) - For unit testing
- CSS Flexbox and Grid
- Semantic HTML
- Open Graph Protocol

### What I learned

- Hide/show navbar depending on scroll direction
- Creating a form component in React
- Creating a controlled component in React
- Creating routes using React Router v6
- Creating unit tests using React Testing Library
- Storing state using localStorage API
- Using aria attributes to ensure my application is accessible to users
- Handling form submission and validation
- Managing state within a component using UseState Hook
- Handling side-effects using useEffect Hook
- Creating a basic list component using map function
- Using keys within list Components
- Lifting state up
- Styling React App with Pure CSS
- Adding Open Graph Protocol meta tags to improve SEO

Here is a code snippet: 

```jsx
const BookingForm = ({ availableTimes, dispatch }) => {
  const navigate = useNavigate();
  const { times } = availableTimes;
  const [bookings, setBookings] = useState({
    date: '',
    time: '17:00',
    guests: '',
    occasion: 'Birthday',
  });

  useEffect(() => {
    localStorage.setItem('Bookings', JSON.stringify(bookings));
  }, [bookings]);
```

### Useful resources

- [React Docs (Rendering Lists) ](https://reactnative.dev/docs/stylesheet) - This helped me for rendering lists in the navbar. I really liked their documentation and will use it going forward.  
- [React Testing Library ](https://testing-library.com/docs/react-testing-library/intro/) - This helped me for creating unit tests in React.
- [React Router (useNavigate)](https://reactrouter.com/en/6.5.0/hooks/use-navigate) - This helped me for redirecting user to a confirmed booking page.
