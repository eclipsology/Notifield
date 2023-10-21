
# Notifield

Notifield is a notification library based on [Rayfield](https://rayfield.dev) by [Sirius](https://sirius.menu)

It is a stripped down, bare-bones version of Rayfield, which features exclusively notifications.

Using Rayfield, you have to start the main UI screen in order to utilize the stylish and modern notification system, which may be a problem for those who don't want a big clunky UI on their screen. For that purpose, I spent a few hours of my time stripping down Rayfield's code, and making it into a single-functioned and easy-to-use library.

# Documentation
To load the UI Library, paste the following at the top of your code:
```lua
loadstring(game:HttpGet("https://raw.githubusercontent.com/eclipsology/Notifield/main/source"))()
```

In order to make a notification, simply use the following code:
```lua
Notify({
        Title = "Notification Title",
        Content = "Notification Description",
        Duration = 4, -- (Seconds)
        Icon = 7536788153, -- Do not include the "rbxassetid://" portion
        Actions = {
            Accept = {
                Name = "Ok",
                Callback = function()
                    print('User Clicked "Ok"')
                end
            },
        }
    })
```

It will end up looking like this:

![Screenshot of Notifield Example Notification](https://github.com/eclipsology/Notifield/blob/main/images/image.png?raw=true)
