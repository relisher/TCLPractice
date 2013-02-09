
proc fib {val} {
set a 1
set b 1
set c 2
if {$val > 0} {
while {$c < $val} {
set a [expr $a+$b]
set b [expr $a+$b]
set c [expr $c+2]
}
if {$c == $val} {
set result $b
}
if {$c == [expr $val+1]} {
set result $a
}
}
if {$val == 0} {
set result 0
}
if {$val < 0} {
set result "Number too low!"
}
return $result
}
entry .value -width 7 -relief sunken -textvariable value
label .description -text "result is:"
label .result -textvariable result
button .calculate -text "Find the fib!" \
    -command {set result [fib $value]}
bind .value <Return> {
    .calculate flash
    .calculate invoke
}
grid .value .description .result -padx 2m -pady 2m
grid .calculate - - -padx 2m -pady 2m
