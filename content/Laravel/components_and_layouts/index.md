---
title: "Components and Layouts"
date: 2025-11-14
weight: 6
---

## Components and Layouts

Now that we have our custom home page set up, let's make it look professional! To do this, we're going to learn about **components**.

### What Are Components?

In web development, a **component** is a reusable piece of code that represents a part of your user interface. Think of components as building blocks - instead of writing the same code over and over again every time you need a button, a form, or a navigation menu, you create it once as a component and then reuse it throughout your application.

For example, imagine you need buttons on 20 different pages. Without components, you'd have to:
- Write the button HTML 20 times
- Style it with CSS 20 times
- If you want to change the button design, update it in 20 different places!

With components, you:
- Create the button component once
- Use it on all 20 pages
- Change the design in one place and it updates everywhere automatically

Components make your code cleaner, more organized, and much easier to maintain!

### Pre-Made Components: The Flux Library

Now, we could build all our components from scratch, but that would take a lot of time and design skill. Instead, we're going to use a library of pre-made components called **Flux** that comes built in to the Livewire Starter Kit we chose earlier.

Flux is a modern UI component library designed specifically for Laravel applications. It provides pre-built components like buttons, forms, navigation menus, and more - all styled and ready to use. This saves us tons of time because we don't have to design and style every element ourselves!

Just like components we create ourselves, Flux components can still be customised - so we can change them to match our theme if we don't want to go with the 'out of the box' look.

### Adding Buttons to Our Home Page

Let's add some professional-looking login and register buttons to our new home page. We'll use Flux's button components which are already nicely styled.

In your `home.blade.php` file, add the following code inside the `<body>` tag underneath your `<h1>` element:

```blade
<div class="flex gap-4">
    <flux:button type="submit" variant="outline" href="{{ url('/login') }}">
        Log in
    </flux:button>

    <flux:button type="submit" variant="primary" href="{{ url('/register') }}">
        Register
    </flux:button>
</div>
```

#### Understanding the Code

Let's break down what this code does:

- **`<div class="flex gap-4">`** - Creates a flexible container with a gap between items (this is using Tailwind CSS, which Flux is built on. If you aren't familiar with divs or classes, be sure to check out our HTML & CSS Tutorial!)
- **`<flux:button>`** - A Flux component that creates a styled button
- **`variant="outline"`** - Makes the login button have an outlined style (border with no fill)
- **`variant="primary"`** - Makes the register button have a filled primary color style
- **`href="{{ url('/login') }}"`** - Sets where the button links to. The `{{ }}` is Blade syntax for outputting PHP code
- **`url('/login')`** - Laravel's helper function that generates the full URL for the login page

### Flux Components vs Regular HTML

Using Flux components like `<flux:button>` instead of regular HTML buttons gives you several benefits:

1. **Consistent styling** - All Flux buttons look the same across your entire application
2. **Built-in variants** - Easy access to different styles (primary, outline, danger, etc.)
3. **Accessibility** - Flux components follow web accessibility best practices
4. **Less code** - You don't need to write CSS classes for every button

Compare this Flux button:
```blade
<flux:button variant="primary">Click me</flux:button>
```

To achieving the same look with regular HTML:
```html
<button class="bg-blue-600 hover:bg-blue-700 text-white font-semibold py-2 px-4 rounded shadow-sm transition-colors duration-150">
    Click me
</button>
```

Much simpler with Flux!

Next: [Working with the Database](/laravel/working_with_database/)
