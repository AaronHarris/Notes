# LA Ruby Meetup - November 2012  
11/7/2012  
Videos Posted to LA Ruby youtube channel: <http://www.youtube.com/user/LosAngelesRuby>  
7:30, THH116

# Executive Summary

## Ruby Made Simple
A series of talks that will be given at each meetup going forward

### What about if?
By Ron Evans, The Hybrid Group, @deadprogram  
There are seven ways to write if statements / conditionals in Ruby

1.  `if some_condition  
      `&nbsp;&nbsp;`do something  
    end`
2.  `if some_condition  
      `&nbsp;&nbsp;`do something  
    else  
      `&nbsp;&nbsp;`do something_else  
    end`
3.  `if some_condition  
      `&nbsp;&nbsp;`do something  
    elsif another_condition  
      `&nbsp;&nbsp;`do something_else  
    else  
      `&nbsp;&nbsp;`do otherwise  
    end`
4.  `unless not_condition  
      `&nbsp;&nbsp;`do something  
    end`
    
    Now how do we make these more consice / better readable?

5.  do something if some_condition
6.  do something unless some_condition
    - ie. raise "error" unless valid?
7.  some_condition ? do_something_true : do_something_false
    - ternary operator

### GitNesse: Acceptance Testing Using Cucumber & Git-wiki
By Ron Evans, The Hybrid Group, @deadprogram

- FitNesse is a wiki to allow business people to enter in their own requirements
    - You are essentially testing executable specifications
- If you're using Cucumber to click buttons, you're doing it wrong.
    - It's to test requirements, not to test the system
- "Round trip" solution engineering, not one-way
    Let users collaboratively use the wiki to make requirements
- **Specification by Example** - best book to learn whether solution is meeting business requirements
- <http://github.com/hybridgroup/gitnesse-demo/wiki>
- <http://gitnesse.com>

### KidsRuby & Sphero
By Ron Evans, The Hybrid Group, @deadprogram

- KidsCodeCamp was held @RubyConf in Denver, CO
- Taught 65 kids how to program using Ruby and robots   
- **Sphero**: a very small spherical bluetooth robot made by Orbotics in Boulder, CO
- The Hybrid Group modified the KidsRuby program to support Sphero programming out of the Box
    - Most of the work was dealing with the Ruby 'Serial' gem
- <gosphero.com>
- <kidsruby.com> - now Sphero compatible out of the box

<http://www.github.com/hybridgroup> - the organization for the projects mentioned above

## JCOv: Coverage Testing your JavaScript
By Doug McInnes, YP (Yellow Pages), dougmcinnes.com  
<http://github.com/dmcinnes>  

- You may have 100% coverage on Ruby code with RSpec
- His project had 8 lines of JavaScript for everty 10 lines of Ruby code
- JavaScript is code too! You need to cover it as much as your Ruby code.
- There have been lots of attempts at automated testing scripts, including JSpec, but they were all abandoned
- His team wrote and open-sources JCov, a headless (w/o browser) JS testing framework
    - Uses TheRubyRacer/V8 engine (very fast)

- `gem install jcov`
- Make ascii flowcharts using <http://asciiflow.com>
- <http://github.com/yp-engineering>

# Test-Driven Development: Write better code in less time
By Evan Dorn, Founder *Logical Reality Design*  
<http://lrdesign.com>

- Intelligence a liability when writing good software
    - Smart people can keep so much stuff in their head, they make progress without a process (This is not a good thing)
- Professionals:
    - Deisgn, plan, and prepare their work
        - then do the work
    - this produces better results faster
- Process:
    - Process is the difference between surgery and cutting people
    - Difference between Engineering and Tinkering
    - Software Engineering vs Programming
- Software Process
    - Architecture
    - Conventions and Standards
    - Version control
    - Coordination (agile)
    - Test-Driven Development
- Tests provide:
    - Documentation of Code
    - Catch future errors
    - Long-term time savings
      - But tests are a tool, not a process.
- TDD defined:
    1. Decide what the code will do
    2. write a test that will pass if the code does that thing
    3. Run the test, see it fail
    4. write your code
    5. Run the test, see it pass
    - If you have to backtest, remove code, see it fail, but code back, see it pass
- TDD Process:
    - Design and plan before you code
    - Document your design
    - Proof that code implements design
    - Encourages design of testable code
- Testable Code:
    - Looks a lot like good code
    - If your test is too long, your method/code is too complex. It needs to do one thing well.
    - Modular
    - Decoulbed design
    - Methods of limited scope
    - strinking in cyclomatic complexity - how many paths there are through the code
        - Every conditional in your program is another test you have to write

- <http://destroyallsoftware.com> - video postcast subscription where guy teaches how to get good with tests
- <http://solvemyword.com> - A project he worked on for his girlfriend, where he spend 1.5 hours trying to make the project on an airplane with no success (messy code, didn't work), then scrapped his project and started over test-first, has better and working code in 35 minutes.

## Table Cloth
By Robert Ross, aka [Bobby Tables](http://xkcd.com/327), Philosophie Software  
Using impress.js for his presentation

- Made 2 table view-helpers, PHP, Ruby  
`<%= simple_table_for @users, with: UserTable %>`
- usually we have to define the specific table code
- What about if certain columns only certain users we want to see? ie. `current_user.admin?`
- `gem install table_cloth`
- a tables/ director in the app/ folder
    - `<%= simple_table_for [Container.new], with: ContainerTable %>`
- You can also define your own presenters, which control how a table is rendered (header, body)
    - You could even generate tables with sort columns, add `using: #{Presenter class you defined}`

- <http://github.com/bobbytables/table_cloth>
- <http://gophilosophie.com>