---
layout: post
title:  "Bash Script Reflection"
date:   2016-11-03
categories: "projects"
assignment: "true"
---
[Link to Github Repository](https://github.com/ldinkins/malily-assignment-4)

Lily and I started off the assignment by trying to figure out what questions we wanted to ask. Surprisingly, this took a while. Then, we tried to generate random strings. We hit a snag with this portion because we didn't know how to save the output of the generator command into a variable. We realized that putting parentheses around the `cat` command would fix the problem. Afterwards, we moved onto creating the datestamp. I realized that the time zone wasn't EST, so I changed the original command to include the time zone. Once that was done, we worked on putting all of the output in a CSV file. Originally, the command rewrote answers in the CSV instead of appending them. After adding an extra `>`, the script appended the CSV instead of rewriting it. That concluded the base requirements for the assignment.

For the bonus portion, Lily and I decided to work on things individually and use pull requests for collaboration. I decided to create a function to print the CSV results to the screen, like in the tutorial from the class notes. It was fairly straightforward, but it wasn't very pretty. Making the names bold made the output look a little bit better, but I thought it could use some color. Lily decided to work on making everything prettier. She added a color scheme that made the questions and output look a lot better. When we were going back and forth to edit things, Lily ran into a conflict that she resolved. Other than that, we didn't have any problems. I think the whole assignment was a cool way to work as a group and use git to make it easier to collaborate.
