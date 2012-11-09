LA Ruby Meetup - November 2012
11/7/2012
Videos Posted to LA Ruby youtube channel: [[http://www.youtube.com/user/LosAngelesRuby]]
7:30, THH116

# Executive Summary

## Ruby Made Simple
- A series of talks that will be given at each meetup going forward

### What about if?
By Ron Evans, The Hybrid Group, @deadprogram
There are seven ways to write if statements / conditionals in Ruby
1.  `if some_condition  
        do something  
    end`
2.  `if some_condition  
        do something  
    else  
        do something_else  
    end`
3.  `if some_condition  
        do something  
    elsif another_condition  
        do something_else  
    else  
        do otherwise  
    end`
4.  `unless not_condition  
        do something  
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
- [[http://github.com/hybridgroup/gitnesse-demo/wiki]]
- [[http://gitnesse.com]]

### KidsRuby & Sphero
By Ron Evans, The Hybrid Group, @deadprogram
- KidsCodeCamp was held @RubyConf in Denver, CO
- Taught 65 kids how to program using Ruby and robots   
- **Sphero**: a very small spherical bluetooth robot made by Orbotics in Boulder, CO
- The Hybrid Group modified the KidsRuby program to support Sphero programming out of the Box
    - Most of the work was dealing with the Ruby 'Serial' gem
- [[gosphero.com]]
- [[kidsruby.com]] - now Sphero compatible out of the box

[[http://www.github.com/hybridgroup]] - the organization for the projects mentioned above

##

