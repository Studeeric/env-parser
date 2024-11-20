# Godot .env parser

This is a simple and easy to use .env parser for your projects.

## Setup

Simply put the `env-parser` folder in your `addons` folder.
Next go add the `env-parser` as a global by doing the following:
`Project` -> `Project Settings...` -> `Globals` -> click on the folder icon and select the `EnvParser.gd` file -> Press `Add`.

By default the project will look for a `.env` file in the root of your project.
If you wish to change that, you can do so by changing the value of the `file_path` variable in the `EnvParser.gd` script.

## Use

Simply call `EnvParser.parse(env_key)`, and it will return a `String` value of whatever your `env_key` has as value in the `.env` file.
In this project there is a simple example.

## Warnings

The project will push an `error` when the `.env` file cannot be found.
The project will push a `warning` when it can't find the value you're looking for or the key is simply empty.

## Last reminder
Make sure to place `.env` in your `.gitignore` file before you upload it. ;)

**Happy coding!**
