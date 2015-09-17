[t]<span>1</span>

![image](zb2l3)

Description {#description .unnumbered}
===========

This is a simple, cheap, standalone battery capacity tester from Ebay (around \$5). It connects to the battery and a load resistor, and draws power from a microUSB connector (no communications to the computer, just power). It draws power from the battery until a predetermined discharge termination voltage is reached, whence it displays the integrated Ampere-hours (Ah) of battery capacity (it’s a pity that Ah is the accepted unit rather than Volt-Ampere-seconds, a.k.a Joules). The Ebay description is hard to understand, so I edited it into more conventional English. All errors therefore are mine—I am uncertain about the details in the calibration section, for instance.

-   External load resistor (7.5 W)

-   Power supply voltage: DC4.5-6V (micro USB interface)

-   Working current: less than 70mA

-   Measured battery voltage: 1.00V-15.00V, resolution 0.01V

-   Automatically selected termination voltage, depending on the initial charged cell voltage (range: 0.5-11.0V)

-   Maximum current 3A, resolution 0.001A

-   The maximum measurement error voltage: 1% +- 0.03V

-   The maximum measurement error of current: 2% +- 0.010A

-   The maximum battery capacity range: 0.001Ah..9999Ah (values lower than 10Ah are displayed as X.XXX; values between 10Ah and 99.99Ah are displayed as XX.XX, and so on).

-   Board size: 50mm long by 36mm wide, by 17mm high, including standoffs

Note: in order to improve the voltage measurement accuracy, the circuit applies a DC bias. The display may show a small residual value, which does not affect the actual measurement.

Usage instructions {#usage-instructions .unnumbered}
==================

1.  Measured battery should be fully charged.

2.  Connect to the tested battery observing the polarity (+ terminal on the PCB to positive battery terminal). ***Reversing The Polarity May Damage The Circuit!*** Connect the operating power to the tester via the micro USB cable. The display should indicate the battery voltage.

3.  Start test by pressing the OK button. The tester will automatically set suitable termination voltage, according to the battery full charge voltage, and flash it 3 times upon starting the test.

    -   The termination voltage chan be changed in 0.1V increments after starting the test, by pressing the + or - keys. The termination voltage is displayed with a leading P character.

4.  During testing, the electronic switch connects the load resistor, and the testing data are displayed in sequence, as shown by the LED indicator:

    -   the integrated capacity (Ah),

    -   instantaneous discharge current (A)

    -   current battery voltage (V)

5.  When the battery voltage reaches the termination voltage, the tester cuts off the load control switch, and displays the capacity (Ah) and rapidly blinks the corresponding LED indicator. Press OK to terminate flashing. Pressing the OK button again returns to power on state, so that another battery can be connected and tested.

The error codes {#the-error-codes .unnumbered}
---------------

<span>Err1:</span>

:   the battery voltage higher than 15V

<span>Err2:</span>

:   the battery voltage is lower than the setting voltage termination

<span>Err3:</span>

:   the battery is unable to withstand the load discharge current (either the internal battery resistance or connector/cable resistance is too large)

<span>Err4:</span>

:   the current is too large (current is more than 3.1A)

Calibration {#calibration .unnumbered}
-----------

Apply USB power and simultaneously press all three buttons to enter the calibration mode and perform the following steps

1.  The first calibration step after entering the calibration displays the 0u0A; short connect both positive and negative input terminal and press the OK button

2.  Next, the display will show J10u; apply 10.00V DC between the input positive and negative terminal and press the OK button again.

3.  The display will show J2.0A; apply 2.0 A DC current between the input terminals and press the OK button to complete the calibration.

If the tester determines that the calibration data is reliable, it will in turn show 4 calibration numbers after completing the procedure; otherwise it will ignore the calibration attempt, discard the data and exit the procedure.

Shipped contents:  {#shipped-contents .unnumbered}
------------------

-   2x 5W 7.5ohm Resistance

-   1x Battery Capacity Tester Board ( USB cable is NOT provided )


