# csc347-ens211-lab-10-latches-and-flip-flops-solved
**TO GET THIS SOLUTION VISIT:** [CSC347-ENS211 Lab 10-Latches and Flip-Flops Solved](https://www.ankitcodinghub.com/product/csc347-ens211-lab-10-latches-and-flip-flops-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;94126&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSC347-ENS211 Lab 10-Latches and Flip-Flops Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<strong>Lab </strong><strong>10 Latches and Flip-Flops </strong>

The objective of this lab is to model and investigate the behavior of various latches and flip-flops.

Sequential circuits are the digital circuits in which the output depends not only on the present input (like combinatorial circuits), but also on the past sequence of inputs. In effect, these circuits must be able to remember something about the past history of the inputs. Thus the timing concept is introduced and the clock signal provides the timing essence to sequential circuits. Latches and flip-flops are memory devices in sequential circuits, and are fundamental building blocks of digital electronics systems used in computers, communications, and many other types of systems. A flip-flop or latch is a circuit that has two stable states and can be used to store state information. The circuit can be made to change state by signals applied to one or more control inputs and will have one or two outputs.

&nbsp;

<strong><u>Laches</u></strong>

Latch is a device with exactly two stable states: high-output and low-output. A latch has a feedback path, so information can be retained by the device. Therefore latches are volatile memory devices, and can store one bit of data for as long as the device is powered. As the name suggests, latches are used to “latch onto” information and hold in place.

&nbsp;

<ol>
<li><strong>SR Latch</strong></li>
</ol>
An SR latch (Set/Reset) is an asynchronous device: it works independently of control signals and relies only on the state of the S and R inputs. The SR Latch a circuit with two cross-coupled NOR gates or two cross-coupled NAND gates, and two inputs labeled S for set and R for reset. The latch has two useful states. When output Q = 1, the latch is said to be in the set state. When Q = 0, it is the reset state. Outputs Q and Q’ are normally the complement to each other. However, when both inputs are equal to 1 at the same time, a condition in when both outputs are equal to 0 (rather than be mutually complementary) occurs. If both inputs are then switched to 0 simultaneously, the device will enter an unpredictable or undefined state. Therefore, setting both inputs to 1 is forbidden. Under normal conditions, both inputs of the latch remain at 0 unless the state has to be changed.

<strong>Procedure</strong><strong>&nbsp;</strong>

<ol>
<li>Crate a Verilog module for the SR Latch using structural(gate)-level modeling</li>
</ol>
<strong>module</strong> SR_latch (R, S, Q, Qprime);

<strong>input</strong> R, S;

<strong>output</strong> Q, Qprime;

nor n0(Q,R,Qprime);

nor n1(Qprime,S,Q);

&nbsp;

<strong>endmodule</strong>

<strong>&nbsp;</strong>

<ol>
<li>Develop a testbench to test and validate the design. You should generate the input stimuli as shown in the below timing diagram.</li>
</ol>
<strong>module test_SR_latch;</strong>

<strong>&nbsp; reg R, S; // inputs</strong>

<strong>&nbsp; wire Q, QPrime; // outputs</strong>

<strong>&nbsp; </strong>

<strong>&nbsp; // module SR_latch (R, S, Q, Qprime);</strong>

<strong>&nbsp; SR_latch uut(R, S, Q, Qprime);</strong>

<strong>&nbsp; </strong>

<strong>&nbsp; initial </strong>

<strong>&nbsp;&nbsp;&nbsp; begin</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $dumpfile(“dump.vcd”);</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $dumpvars(1, test_SR_latch);</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; // display the inputs and outputs</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $monitor(“R=%b S=%b Q=%b Q’=%b”, S, R, Q, Qprime);</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; R = 0; S = 0;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 R = 0; S = 1;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 R = 0; S = 0;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 R = 1; S = 0;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 R = 1; S = 1;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 $finish</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong>

<strong>&nbsp;&nbsp;&nbsp; end</strong>

&nbsp;

<ol start="2">
<li><strong>D Latch </strong></li>
</ol>
The D latch (D for “data”) or transparent latch is a simple extension of the gated SR latch that removes the possibility of invalid input states (metastability). Since the gated SR latch allows us to latch the output without using the S or R inputs, we can remove one of the inputs by driving both the Set and Reset inputs with a complementary driver, i.e. we remove one input and automatically make it the inverse of the remaining input. The D latch outputs the D input whenever the C (Control/Enable) line is high, otherwise the output is whatever the D input was when the C input was last high. This is why it is also known as a transparent latch – when C is asserted, the latch is said to be “transparent” – it signals propagate directly through it as if it isn’t there.

&nbsp;

<table>
<tbody>
<tr>
<td width="0"></td>
<td width="246"></td>
<td width="36"></td>
<td width="187"></td>
</tr>
<tr>
<td></td>
<td rowspan="2"></td>
</tr>
<tr>
<td></td>
<td></td>
<td rowspan="2"></td>
</tr>
<tr>
<td></td>
</tr>
</tbody>
</table>
&nbsp;

<strong>Procedure</strong>

<ol>
<li>Model the D Latch in behavioral modeling</li>
</ol>
<strong>module D_Latch (D, C, Q, Qprime);</strong>

<strong>&nbsp; input D, C;</strong>

<strong>&nbsp; output Q, Qprime;</strong>

<strong>&nbsp; // redeclare Q AND Q’ TO BE THE TYPE OF REG</strong>

<strong>&nbsp; reg Q = 0, Qprime;</strong>

<strong>&nbsp; </strong>

<strong>&nbsp; always @ (D or C)</strong>

<strong>&nbsp;&nbsp;&nbsp; begin</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if (C)</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Q &lt;= D;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Qprime &lt;= ~D;</strong>

<strong>&nbsp;&nbsp;&nbsp; end</strong>

<strong>endmodule</strong>

<ol>
<li>Develop a testbench to test and validate the design. You should generate the input stimuli as shown in the below timing diagram.</li>
</ol>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; module test_D_Latch;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; reg&nbsp; D, C;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; wire Q, QPrime;&nbsp;&nbsp;&nbsp; </strong>

<strong>&nbsp;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; // module D_Latch (D, C, Q, Qprime);</strong>

<strong>&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;D_Latch uut(D, C, Q, QPrime)</strong>

<strong>&nbsp;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; initial </strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; begin</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp; $dumpfile(“dump.vcd”);&nbsp; </strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $dumpvars(1, test_D_Latch);&nbsp; </strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; // display the inputs and outputs</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $monitor( “D=%b&nbsp; C=%b&nbsp; Q=%b&nbsp; Q’=%b”, D,C,Q,QPrime);</strong>

<strong>&nbsp;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;C=0; D=0;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 C=0; D=1;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 C=1; D=0;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 C=1; D=1;</strong>

<strong>&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;#10 $finish;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; end</strong>

<strong>&nbsp;&nbsp;&nbsp; endmodule</strong>

&nbsp;

<strong><u>Flip-Flops</u></strong>

Flip-flops are clocked circuits whose output may change on an active edge of the clock signal based on its input. Unlike latches, which are transparent and in which output can change when the gated signal is asserted upon the input change, flip-flops normally would not change the output upon input change even when the clock signal is asserted. Flip-flops are widely used in synchronous circuits.

&nbsp;

<ol>
<li><strong>D Flip-Flop</strong></li>
</ol>
The D flip-flop is a widely used type of flip-flop. It is also known as a data or delay flip-flop. The D flip-flop captures the value of the D-input at a definite portion of the clock cycle (such as the rising edge of the clock). That captured value becomes the Q output. At other times, the output Q does not change. The D flip-flop can be viewed as a memory cell or a delay line. The active edge in a flip-flop could be rising or falling. The following figure shows rising (also called positive) edge triggered D flip-flop and falling (negative edge) triggered D flip-flop.

<table>
<tbody>
<tr>
<td width="0"></td>
<td width="217"></td>
<td width="66"></td>
<td width="93"></td>
</tr>
<tr>
<td></td>
<td colspan="2"></td>
<td rowspan="3"></td>
</tr>
<tr>
<td></td>
<td></td>
</tr>
<tr>
<td></td>
</tr>
</tbody>
</table>
&nbsp;

<strong>Procedure</strong>:

&nbsp;

<ol>
<li>Crate a Verilog module for a rising edge triggered D flip-flop in behavioral modeling</li>
</ol>
<strong>module D_ff (Clk, D, Q, Qprime);</strong>

<strong>&nbsp; input Clk, D;</strong>

<strong>&nbsp; output reg Q, Qprime;</strong>

<strong>&nbsp; </strong>

<strong>&nbsp; always @ (posedge Clk)</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; begin</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Q &lt;= D;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Qprime &lt;= ~D;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; end</strong>

<strong>endmodule</strong>

&nbsp;

<ol>
<li>Develop a testbench to test and validate the design. You should generate the input stimuli as shown in the below timing diagram.</li>
</ol>
module testDFF;

reg&nbsp; Clk, D;

wire Q, Qprime;

&nbsp;

D_ff uut(Clk, D, Q, Qprime);

&nbsp;

// generate the clock signal

initial

begin

Clk = 0;

forever&nbsp; #5 Clk = ~Clk;

#200 $finish;

end

&nbsp;

initial

begin

$dumpfile(“dump.vcd”);

$dumpvars(1, testDFF);

// display the inputs and outputs

$monitor( “Clk = %b&nbsp; D = %b&nbsp; Q = %b&nbsp; Q’ = %b”, Clk,D,Q,Qprime);

D=0;

#10 D = 1;

#10 D = 0;

#10 D = 1;

#10 D = 0;

#10 D = 1;

#10 D = 0;

&nbsp;

#10 $finish;

end

endmodule

<ul>
<li><strong>D Flip-Flop with Set/Reset</strong></li>
</ul>
Often it is necessary to have the synchronous element to start with a defined output. It is also desired and required in some circuits to force the synchronous element to a known output ignoring input at the D input. The D flip-flop discussed above can be modified to have such functionality. Such D flip-flop is known as D flip-flop with synchronous set and reset capabilities if the desired output is obtained on the active edge of the clock, otherwise it is viewed to have asynchronous preset and clear. The model of the DFF with synchronous reset is shown below.

&nbsp;

<strong>module</strong> D_ff_with_synch_reset (D, Clk, reset, Q, Qprime);

<strong>input</strong> D, Clk, reset;

<strong>output</strong> Q, Qprime;

<strong>reg</strong> Q =0, Qprime;

&nbsp;

<strong>always</strong> @(<strong>posedge</strong> Clk)

<strong>if</strong> (reset)

<strong>begin</strong>

Q &lt;= 1’b0;

Qprime &lt;= 1’b1;

<strong>end</strong>

<strong>else</strong>

<strong>begin</strong>

Q &lt;= D;

Qprime &lt;= ~D;

<strong>end</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; endmodule</strong>

&nbsp;

&nbsp;

<strong>Procedure</strong>:

Develop a testbench to test and validate the design. You should generate the input stimuli as shown in the below timing diagram. <strong>You can simply copy the test cases for the DFF above and then add the test cases for the reset. </strong>

<strong>module test_Dff_with_synch_reset;</strong>

<strong>&nbsp; reg D, Clk, reset;</strong>

<strong>&nbsp; wire Q, Qprime;</strong>

<strong>&nbsp; </strong>

<strong>&nbsp; D_ff_with_synch_reset uut(D, Clk, reset, Q, Qprime);</strong>

<strong>&nbsp; </strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp; initial</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; begin</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp; Clk = 0;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp; forever&nbsp; #5 Clk = ~Clk; </strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #200 $finish;&nbsp; </strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; end </strong>

<strong>&nbsp;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; initial</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; begin</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp; $dumpfile(“dump.vcd”);&nbsp; </strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $dumpvars(1, test_Dff_with_synch_reset);&nbsp; </strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $monitor( “D = %b&nbsp; Clk = %b&nbsp; reset = %b&nbsp; Q = %b&nbsp; Q’ = %b”, D, Clk, reset, Q, Qprime);</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; D = 0; reset = 0; </strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 D= 1;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 D=0;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 D = 1; reset = 1;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 D = 0;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 D = 1;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 D = 0;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 D = 1; reset = 0;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; D = 0;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 $finish;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; end</strong>

<strong>endmodule</strong>

&nbsp;

<strong><u>Submission Instructions:</u></strong>

<u>Lab work submission</u>

<ol>
<li>Take screenshots of all your waveforms.</li>
<li>Add the following information as comments to the beginning of your code. Make sure to click the “Save” button to save your project, then take a screenshot of your code.</li>
</ol>
// Author:&nbsp;&nbsp;&nbsp; Name

// Lab 10:&nbsp; put the title here

// Link to your project

&nbsp;

<ol start="3">
<li>Copy the link of your design from the address bar of the browser.</li>
<li>On the Blackboard, click on Lab 10. Attach the screenshot from the first two steps and paste the link from Step 3 into the Comments area, then click the “Submit” button.</li>
</ol>
&nbsp;

&nbsp;

<table>
<tbody>
<tr>
<td width="671">// Author: Gianna Rose

// Lab 10

// https://www.edaplayground.com/x/NLTd

&nbsp;

// module test_SR_latch;

//&nbsp;&nbsp; reg R, S;

//&nbsp;&nbsp; wire Q, Qprime;

&nbsp;

//&nbsp;&nbsp; // module SR_latch (R, S, Q, Qprime);

//&nbsp;&nbsp; SR_latch uut(R, S, Q, Qprime);

&nbsp;

//&nbsp;&nbsp; initial

//&nbsp;&nbsp;&nbsp;&nbsp; begin

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $dumpfile(“dump.vcd”);

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $dumpvars(1, test_SR_latch);

&nbsp;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; // display the inputs and outputs

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $monitor(“R = %b S = %b Q = %b Q’ = %b”, S, R, Q, Qprime);

&nbsp;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; R = 0; S = 0;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 R = 0; S = 1;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 R = 0; S = 0;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 R = 1; S = 0;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 R = 1; S = 1;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 $finish;

&nbsp;

//&nbsp;&nbsp;&nbsp;&nbsp; end

// endmodule

&nbsp;

// OUTPUT

// R = 0 S = 0 Q = x Q’ = x

// R = 1 S = 0 Q = 1 Q’ = 0

// R = 0 S = 0 Q = 1 Q’ = 0

// R = 0 S = 1 Q = 0 Q’ = 1

// R = 1 S = 1 Q = 0 Q’ = 0

&nbsp;

// ————————————————–

&nbsp;

// &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; module test_D_Latch;

// &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; reg&nbsp; D, C;

// &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; wire Q, Qprime;

&nbsp;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; // module D_Latch (D, C, Q, Qprime);

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; D_Latch uut(D, C, Q, Qprime);

&nbsp;

// &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; initial

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; begin

// &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;$dumpfile(“dump.vcd”);

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $dumpvars(1, test_D_Latch);

&nbsp;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; // display the inputs and outputs

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $monitor( “D = %b&nbsp; C = %b&nbsp; Q = %b&nbsp; Q’ = %b”, D, C, Q, Qprime);

&nbsp;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;C=0; D=0;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 C = 0; D = 1;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 C = 1; D = 0;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 C = 0; D = 0;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 C = 1; D = 1;

//&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;#10 $finish;

&nbsp;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; end

//&nbsp;&nbsp;&nbsp;&nbsp; endmodule

// OUTPUT

// D = 0&nbsp; C = 0&nbsp; Q = 0&nbsp; Q’ = x

// D = 1&nbsp; C = 0&nbsp; Q = 0&nbsp; Q’ = x

// D = 0&nbsp; C = 1&nbsp; Q = 0&nbsp; Q’ = 1

// D = 0&nbsp; C = 0&nbsp; Q = 0&nbsp; Q’ = 1

// D = 1&nbsp; C = 1&nbsp; Q = 1&nbsp; Q’ = 0

&nbsp;

// ————————————————–

&nbsp;

//&nbsp;&nbsp;&nbsp; module testDFF;

// &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; reg&nbsp; Clk, D;

// &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; wire Q, Qprime;

&nbsp;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; D_ff uut(Clk, D, Q, Qprime);

&nbsp;

//&nbsp;&nbsp;&nbsp; // generate the clock signal

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; initial

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; begin

// &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;Clk = 0;

// &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;forever&nbsp; #5 Clk = ~Clk;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #200 $finish;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; end

&nbsp;

// &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; initial

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; begin

// $dumpfile(“dump.vcd”);

// $dumpvars(1, testDFF);

// &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;// display the inputs and outputs

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $monitor( “Clk = %b&nbsp; D = %b&nbsp; Q = %b&nbsp; Q’ = %b”, Clk, D, Q, Qprime);

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; D=0;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 D = 1;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 D = 0;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 D = 1;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 D = 0;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 D = 1;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 D = 0;

&nbsp;

//&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;#10 $finish;

//&nbsp;&nbsp;&nbsp;&nbsp; end

// endmodule

&nbsp;

// OUTPUT

// Clk = 0&nbsp; D = 0&nbsp; Q = x&nbsp; Q’ = x

// Clk = 1&nbsp; D = 0&nbsp; Q = 0&nbsp; Q’ = 1

// Clk = 0&nbsp; D = 1&nbsp; Q = 0&nbsp; Q’ = 1

// Clk = 1&nbsp; D = 1&nbsp; Q = 1&nbsp; Q’ = 0

// Clk = 0&nbsp; D = 0&nbsp; Q = 1&nbsp; Q’ = 0

// Clk = 1&nbsp; D = 0&nbsp; Q = 0&nbsp; Q’ = 1

// Clk = 0&nbsp; D = 1&nbsp; Q = 0&nbsp; Q’ = 1

// Clk = 1&nbsp; D = 1&nbsp; Q = 1&nbsp; Q’ = 0

// Clk = 0&nbsp; D = 0&nbsp; Q = 1&nbsp; Q’ = 0

// Clk = 1&nbsp; D = 0&nbsp; Q = 0&nbsp; Q’ = 1

// Clk = 0&nbsp; D = 1&nbsp; Q = 0&nbsp; Q’ = 1

// Clk = 1&nbsp; D = 1&nbsp; Q = 1&nbsp; Q’ = 0

// Clk = 0&nbsp; D = 0&nbsp; Q = 1&nbsp; Q’ = 0

// Clk = 1&nbsp; D = 0&nbsp; Q = 0&nbsp; Q’ = 1

// Clk = 0&nbsp; D = 0&nbsp; Q = 0&nbsp; Q’ = 1

&nbsp;

// ————————————————–

&nbsp;

// module test_Dff_with_synch_reset;

//&nbsp;&nbsp; reg D, Clk, reset;

//&nbsp;&nbsp; wire Q, Qprime;

&nbsp;

//&nbsp;&nbsp; D_ff_with_synch_reset uut(D, Clk, reset, Q, Qprime);

&nbsp;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; initial

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; begin

// &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;Clk = 0;

// &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;forever&nbsp; #5 Clk = ~Clk;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #200 $finish;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; end

&nbsp;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; initial

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; begin

// &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;$dumpfile(“dump.vcd”);

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $dumpvars(1, test_Dff_with_synch_reset);

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $monitor( “D = %b&nbsp; Clk = %b&nbsp; reset = %b&nbsp; Q = %b&nbsp; Q’ = %b”, D, Clk, reset, Q, Qprime);

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; D = 0; reset = 0;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 D= 1;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 D=0;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 D = 1; reset = 1;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 D = 0;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 D = 1;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 D = 0;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 D = 1; reset = 0;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10&nbsp;&nbsp;&nbsp;&nbsp; D = 0;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 $finish;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; end

// endmodule

&nbsp;

// OUTPUT

// D = 0&nbsp; Clk = 0&nbsp; reset = 0&nbsp; Q = 0&nbsp; Q’ = x

// D = 0&nbsp; Clk = 1&nbsp; reset = 0&nbsp; Q = 0&nbsp; Q’ = 1

// D = 1&nbsp; Clk = 0&nbsp; reset = 0&nbsp; Q = 0&nbsp; Q’ = 1

// D = 1&nbsp; Clk = 1&nbsp; reset = 0&nbsp; Q = 1&nbsp; Q’ = 0

// D = 0&nbsp; Clk = 0&nbsp; reset = 0&nbsp; Q = 1&nbsp; Q’ = 0

// D = 0&nbsp; Clk = 1&nbsp; reset = 0&nbsp; Q = 0&nbsp; Q’ = 1

// D = 1&nbsp; Clk = 0&nbsp; reset = 1&nbsp; Q = 0&nbsp; Q’ = 1

// D = 1&nbsp; Clk = 1&nbsp; reset = 1&nbsp; Q = 0&nbsp; Q’ = 1

// D = 0&nbsp; Clk = 0&nbsp; reset = 1&nbsp; Q = 0&nbsp; Q’ = 1

// D = 0&nbsp; Clk = 1&nbsp; reset = 1&nbsp; Q = 0&nbsp; Q’ = 1

// D = 1&nbsp; Clk = 0&nbsp; reset = 1&nbsp; Q = 0&nbsp; Q’ = 1

// D = 1&nbsp; Clk = 1&nbsp; reset = 1&nbsp; Q = 0&nbsp; Q’ = 1

// D = 0&nbsp; Clk = 0&nbsp; reset = 1&nbsp; Q = 0&nbsp; Q’ = 1

// D = 0&nbsp; Clk = 1&nbsp; reset = 1&nbsp; Q = 0&nbsp; Q’ = 1

// D = 1&nbsp; Clk = 0&nbsp; reset = 0&nbsp; Q = 0&nbsp; Q’ = 1

// D = 1&nbsp; Clk = 1&nbsp; reset = 0&nbsp; Q = 1&nbsp; Q’ = 0

// D = 0&nbsp; Clk = 0&nbsp; reset = 0&nbsp; Q = 1&nbsp; Q’ = 0

// D = 0&nbsp; Clk = 1&nbsp; reset = 0&nbsp; Q = 0&nbsp; Q’ = 1

// D = 0&nbsp; Clk = 0&nbsp; reset = 0&nbsp; Q = 0&nbsp; Q’ = 1

&nbsp;
</td>
</tr>
</tbody>
</table>
&nbsp;

<table>
<tbody>
<tr>
<td width="671">// Author: Gianna Rose

// Lab 10

// https://www.edaplayground.com/x/NLTd

&nbsp;

module SR_latch (R, S, Q, Qprime);

input R, S;

output Q, Qprime;

nor n0(Q,R,Qprime);

nor n1(Qprime,S,Q);

&nbsp;

endmodule

&nbsp;

module D_Latch (D, C, Q, Qprime);

input D, C;

output Q, Qprime;

reg Q = 0, Qprime;

&nbsp;

always @ (D or C)

begin

if (C) begin

Q &lt;= D;

Qprime &lt;= ~D;

end

end

endmodule

&nbsp;

module D_ff (Clk, D, Q, Qprime);

input Clk, D;

output reg Q, Qprime;

&nbsp;

always @ (posedge Clk)

begin

Q &lt;= D;

Qprime &lt;= ~D;

end

endmodule

&nbsp;

&nbsp;

module D_ff_with_synch_reset (D, Clk, reset, Q, Qprime);

input D, Clk, reset;

output Q, Qprime;

reg Q =0, Qprime;

&nbsp;

always @(posedge Clk)

if (reset)

begin

Q &lt;= 1’b0;

Qprime &lt;= 1’b1;

end

else

begin

Q &lt;= D;

Qprime &lt;= ~D;

end

endmodule
</td>
</tr>
</tbody>
</table>
&nbsp;

<strong>You do not need to write a lab report for this lab but do the following homework and submit the screenshots and the link to the Blackboard under Lab 10 report submission. </strong>It is due one week after the lab is done.

<strong>Homework</strong>: the following circuit and timing diagrams illustrate the differences between D-latch, rising edge triggered D flip-flop, falling edge triggered D flip-flop, T flip-flop, and JK flip-flop (the input K hardwired to 1). Write Verilog design codes and a testbench to reproduce the following waveforms. You need to initialize Q to 0 at the declaration (e.g. reg Q = 0;) for each flip-flop module. You can test all the flip-flops at once in one testbench.

&nbsp;

<table>
<tbody>
<tr>
<td width="0"></td>
<td width="13"></td>
<td width="123"></td>
<td width="368"></td>
</tr>
<tr>
<td></td>
<td colspan="3"></td>
</tr>
<tr>
<td></td>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>
&nbsp;

&nbsp;

Q<sub>a</sub> = D (if C = 1)

&nbsp;

Q<sub>b</sub> = D&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (positive edge triggered)

&nbsp;

Q<sub>c</sub> = D (negative edge triggered)

&nbsp;

Q<sub>d</sub> = T Å Q<sub>d</sub> (positive edge triggered)

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong>

Q<sub>e</sub> = J Q<sub>e</sub><sup>’</sup> + K’ Q<sub>e</sub> (positive edge triggered), K =1

<strong>&nbsp;</strong>

&nbsp;
