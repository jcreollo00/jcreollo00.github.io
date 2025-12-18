---
layout: essay
type: essay
title: "SWE: Testing Myself Beyond Code"
# All dates must be YYYY-MM-DD format!
date: 2025-12-17
published: true
labels:
  - Software Engineering
  - Agile Project Management
  - Coding Standards
  - User Interface Frameworks
---

<img width="200px" class="rounded float-start pe-4" src="../img/swe.jpg">

## Introduction

When I first started ICS 314, I honestly thought it was just going to be a class about building websites. We learned Next.js, React, PostgreSQL, and built RateMyTools for our final project. But looking back now, the class was teaching me something way bigger than just how to code a website. The real lessons were about software engineering concepts that apply to pretty much any kind of development, not just web apps. Three things that really stuck with me were Agile Project Management, Coding Standards, and User Interface Frameworks. These aren't just web tools - they're approaches I can use no matter what kind of projects I work on later.

## Agile Project Management and IDPM

Agile Project Management is basically a way of organizing software development where you break work into small pieces and work in short cycles instead of planning everything upfront. You build something small, test it, get feedback, and improve it. It's way more flexible than trying to design everything perfectly before you start coding.

In this class we used Issue Driven Project Management, or IDPM. The way it works is you break your project into specific issues - concrete tasks that need to get done. Each issue goes on a project board (we used GitHub Projects), and team members pick up issues, work on them, and mark them done. The key is keeping each issue small enough to finish in a few days, and grouping issues into milestones that represent major stages.

What's cool about IDPM is it's not just for web development. I could totally use this for completely different projects. Like if I was building a machine learning model to predict student performance, I could break it into issues like "collect and clean dataset," "implement baseline model," "test different features," and "optimize parameters." Each one would be an issue on my board, tracked through milestones like "Data Prep," "Model Development," and "Deployment."

The beauty of IDPM is it forces you to think concretely about what needs to be done instead of getting overwhelmed. When we were building RateMyTools, having clear issues made coordination so much easier. We all knew what everyone was working on and could see actual progress. This same approach would work just as well for game development, embedded systems, or literally any software project where you need to manage complexity and work with other people.

## Coding Standards

Coding standards are rules about how to write code - things like how to name variables, format your code, where to put brackets, how to organize imports. At first they seemed annoying, like why does it matter where I put brackets? But after using ESLint all semester, I get why they matter.

The main reason is consistency and readability. When everyone follows the same standards, code looks like one person wrote it even if ten people worked on it. This makes it way easier to read someone else's code and find bugs. We used ESLint to enforce standards for JavaScript - it would flag stuff like unused variables, weird spacing, or missing semicolons, and we had to fix them before merging code.

But coding standards aren't specific to JavaScript or web dev. Every language and every project benefits from having standards. If I was writing Python for data science, I'd follow PEP 8. If I was writing C++ for systems programming, I'd follow Google's C++ style guide. The specific rules change, but the principle stays the same - consistent code is better code.

Beyond formatting, coding standards include best practices that help avoid bugs. Things like "don't use global variables unnecessarily" or "keep functions short" or "use meaningful names" apply no matter what you're building. Whether I'm making a web app, writing automation scripts, or creating a game, following standards makes my code better and easier to work with.

## User Interface Frameworks

A User Interface Framework is basically a collection of pre-built components and design patterns that help you create interfaces faster. We learned Bootstrap 5 and React. Bootstrap gave us ready-made stuff like navigation bars, buttons, and grid layouts. React gave us a way to build interactive interfaces using reusable components.

UI frameworks seem like they're only for web development, and yeah, Bootstrap specifically is for web. But the broader concept applies to any software with a user interface. Instead of building everything from scratch, you use pre-built components for common patterns. This speeds things up and lets you focus on the unique parts of your app.

If I was building a desktop app, I might use Qt or Electron. For a mobile app, React Native or Flutter. For data visualization, D3.js or Plotly. The specific framework changes, but the concept stays the same - use tested components to build faster and more reliably.

What really hit me about React was learning to think about UIs in terms of components and state. A component is a self-contained piece that manages its own data. State is data that changes and makes the UI update. This way of thinking isn't just for web apps - it's how you approach building any interactive system.

Even for non-visual stuff, these principles apply. If I was building a command-line tool, I could still think in terms of components (different commands) and state (current configuration). The framework gives you structure for organizing code and handling complexity, which matters regardless of what kind of interface you're building.

## Conclusion

ICS 314 taught me way more than just web development. Yeah, I can build a full-stack app now with Next.js and PostgreSQL, and that's useful. But the bigger takeaway is understanding software engineering concepts I'll use throughout my career, no matter what I'm building.

Agile and IDPM gave me a framework for breaking down projects and managing work. Coding standards taught me that consistent code is essential for working on teams. UI frameworks showed me how to leverage existing tools and think in terms of components. The specific tech stack we used might change in five years, but these fundamental concepts will still be relevant. That's what makes this class valuable - it wasn't really about learning Next.js, it was about learning to be a software engineer.
