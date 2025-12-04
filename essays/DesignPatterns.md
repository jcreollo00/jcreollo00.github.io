---
layout: essay
type: essay
title: "The Recipe for Better Code: Understanding Design Patterns"
# All dates must be YYYY-MM-DD format!
date: 2025-12-03
published: true
labels:
  - Software Engineering
  - Design Patterns
  - Web Development
  - NextAuth
---

<img width="300px" class="rounded float-start pe-4" src="../img/design-patterns.png">

## Introduction

Design patterns within technology are often considered a blueprint for solving different coding problems that some software engineers may experience. They are similar to recipes within cooking, or blueprints prior to developing something in architecture. They provide many repeatable solutions that can be applied to different situations. Whether an engineer needs faster development or an improvement within code quality, a design pattern can be a proven way to fix these problems by preventing the developer from having to "reinvent the wheel". However, one thing to note is that it isn't just code you can copy-paste, but rather an approach to solving problems. They represent collective wisdom from previous experienced developers. Rather than struggling by yourself, those software engineers before you have refined it and created a sort of plan for you.

## The Language of Patterns

Within software engineering, we use our own 'techniques' which are also known as design patterns. They're not snippets of code you copy and paste, but again approaches to solving recurring problems. When you need to ensure only one instance of a class exists, you use the Singleton pattern. When you need to create objects without specifying their exact types, you can use the Factory pattern. The beauty of design patterns isn't that they make coding easier, but they make it very communicable. When I tell another developer that I "used an Observer pattern here", they can immediately recognize and understand the structure without reading every line. It is essentially like telling a musician 'this is a blues progression'—they will know exactly what to expect.

## Building RateMyTools

When my team and I began building RateMyTools, our platform for UH students to review educational tools and AI resources, I found myself in a similar position to that of a line cook who suddenly was asked to design a menu. I knew the basic ingredients like React, Next.js, and PostgreSQL, but I was unsure how to combine them into a cohesive system. This is where many issues stemmed, specifically when we needed the authentication system to work. Users needed to sign up, log in, maintain sessions across pages, and access protected routes, all while keeping their data secure. I could have built everything from scratch, but instead I turned to NextAuth.js, which implements several crucial design patterns that solved these problems elegantly.

## The Singleton Pattern

Some patterns within the project we noticed were hiding in plain sight. Every time a user logged in, my application needed to talk to the database. But creating a new database connection for every request would be like hiring a new chef for every dish—that would just be chaotic. So this is where Singleton comes in and ensures one Prisma client instance is shared across all requests, reducing connection overhead, improving performance, and preventing database connection errors. Just like the chef example, the Singleton pattern gave us one reliable source of truth.

## The Observer Pattern

Another pattern that emerged naturally was the Observer pattern. When a user logs in, multiple parts of the application need to know about it—the navigation bar needs to show their profile, protected routes need to grant access, and the UI needs to update. The Observer pattern orchestrated this symphony of updates automatically through React's state management. Components using the useSession hook automatically re-render when the authentication state changes, without me writing manual notification code. It's like a head chef calling out orders to the entire kitchen—everyone knows what to do without individual instructions.

## Recognizing Patterns Everywhere

Looking back at the RateMyTools codebase, I started seeing patterns everywhere I hadn't noticed before. That authentication middleware? Strategy pattern. The way React components are structured? Component pattern. Prisma's abstraction layer? Repository pattern. The real revelation came when discussing a bug with a teammate—I mentioned "the issue is with our Singleton database connection" and they immediately understood without seeing any code. That's when I realized design patterns aren't just about writing better code; they're about communicating better with other developers.

## Conclusion

Hopefully using cooking examples simplifies the complexity of design patterns and demonstrates how someone who is new to coding can be transformed into someone who can work in any environment simply by understanding these patterns. Design patterns have ultimately transformed how I approach software development entirely. I have a repertoire of proven solutions, a vocabulary to discuss them, and wisdom to know when to use each one. As I finalize my project for this ICS 314 class, I can already tell my development skills have improved drastically since becoming knowledgeable about design patterns. The patterns are written; now all I need to do is continue the process.
