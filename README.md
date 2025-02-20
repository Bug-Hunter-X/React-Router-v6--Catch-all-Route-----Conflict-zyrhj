# React Router v6 Catch-all Route Conflict

This repository demonstrates a common issue in React Router v6 where the catch-all route (`*`) interferes with other defined routes.  The problem arises when the catch-all route is not placed last in the `Routes` component.

## Problem

Placing the catch-all route before other routes causes it to match all paths, preventing other routes from ever being accessed.  This leads to unexpected behavior and a broken navigation experience.

## Solution

The solution is simple: always place your catch-all route (`*`) as the last route defined within the `Routes` component.  This ensures that React Router attempts to match other routes before falling back to the catch-all.

## Setup

1. Clone the repository.
2. Navigate to the project directory.
3. Run `npm install` to install dependencies.
4. Run `npm start` to start the development server.
