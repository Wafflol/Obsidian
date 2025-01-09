#### calling a function:
bl - address
blr - register

#### function arguments
x0-x7, then stack

#### function results
x0
more results: x1-x7, stack
indirect: x8

#### return address
lr - x30

#### who saves registers
caller save: x0-x18
callee save: x19-x30

#### where stack
sp, aligned on 16B boundary - has to be divisible by 16
grows towards lower addrs
