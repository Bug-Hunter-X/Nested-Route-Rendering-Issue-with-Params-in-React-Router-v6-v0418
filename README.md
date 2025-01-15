# React Router v6 Nested Route Bug

This repository demonstrates a bug encountered when using nested routes in React Router v6.  The issue arises when a parent route includes parameters, causing child routes to fail to render correctly.

## Bug Description

The `User` component, intended to display user details based on an ID parameter, does not render.  This occurs despite proper route definition and parameter access within the component.

## How to Reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.
4. Navigate to `/users/1` (or any other user ID).  The User component should render but does not.

## Solution

The solution involves using the `useParams` hook correctly within the nested components to access route parameters.