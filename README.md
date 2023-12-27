# EditForm Issue

This repo simulates the scenario I encountered when developing my application with Blazor SSR.

# Guidelines

The project is a simple application with a `SearchBar` and a `LoginForm` components, each with an `EditFrom` inside.
The `LoginForm` is used inside the `Home.razor` file, while the `SearchBar` is common to each page and used in the `MailLayout.razor` file.

When used together, I get the following exception:
> InvalidOperationException: EditForm requires either a Model parameter, or an EditContext parameter, please provide one of these.

Meanwhile when I use them separately everything works fine.
To test this behaviour, go in the `Home.razor` and `MainLayout.razor` files and play around by commenting and uncommenting the statements I specified.