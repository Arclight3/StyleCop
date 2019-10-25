# StyleCop MSBuild configuration & Rules
===========================

This repository includes a MSBuild custom configuration file that will add StyleCop Analyzers for each project in a solution. It also contains a ruleset to be used by StyleCop Analyzers.

By adding StyleCop Analyzers within a MSBuild custom configuration file you have the benefit that you're not polluting your projects with configuration.
If you decide later that you want to remove StyleCop, you just have to delete two things from your solution folder and you're done.

## How to use

### Add
* Copy the **Directory.Build.props** file and the **StyleCop** folder in the same directory with your solution file.
* Build your solution.
* That's it! You have enabled StyleCop Analyzers for your solution.

### Remove
* Remove the **Directory.Build.props** file and the **StyleCop** folder from your solution directory.

## How to customize
In the **StyleCop/CustomRules.ruleset** file you can add other rules or you can change the action (None, Warning, Error) for the existing rules.
