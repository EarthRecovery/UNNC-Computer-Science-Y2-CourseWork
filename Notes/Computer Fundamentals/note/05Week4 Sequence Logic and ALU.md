# Sequence Logic and ALU

### Memory

Implementation of memory elements involves synchronization,  clocking and feedback loops

### Clock

The hardware implementation is based on an **oscillator** that  alternates between the beginning phases labelled:

The elapsed time between the beginning of a tick and the end of a subsequent tock is called a **cycle**

![QQ截图20221018163548](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Computer Fundamentals (COMP1036 UNNC)\assets\QQ截图20221018163548.png)

### Flip Flops

**Data Flip Flop** (DFF): the simplest **state keeping** gate (built-in)

 The gate outputs its previous input: out(*t*)= in(*t*-1)

![QQ截图20221018164535](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Computer Fundamentals (COMP1036 UNNC)\assets\QQ截图20221018164535.png)

![QQ截图20221018164112](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Computer Fundamentals (COMP1036 UNNC)\assets\QQ截图20221018164112.png)

### Data and Time in DFF

out(*t*)= in(*t*-1)

• **in** is the gate’s input value

• **out** is the gate’s output value

• **t** is the current clock cycle

• **t-1** is the previous clock cycle

• **t+1** is the next clock cycle

> This elementary behavior can form the basis of all the hardware devices that computers use to maintain state

### Sequential Chips