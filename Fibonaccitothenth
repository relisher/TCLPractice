puts "Enter n to see the nth fibonacci number"
proc fib {n} {
set a 1
set b 1
set c 2
if {$n > 0} {
while {$c < $n} {
set a [expr $a+$b]
set b [expr $a+$b]
set c [expr $c+2]
}
if {$c == $n} {
puts $b
}
if {$c == [expr $n+1]} {
puts $a
}
}
if {$n == 0} {
puts 0
}
if {$n < 0} {
puts "Number too low!"
}
}
