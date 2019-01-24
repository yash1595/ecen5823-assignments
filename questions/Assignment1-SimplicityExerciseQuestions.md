Please include your answers to the questions below with your submission, entering into the space below each question
See [Mastering Markdown](https://guides.github.com/features/mastering-markdown/) for github markdown formatting if desired.

**1. How much current does a single LED draw when the output drive is set to "Strong" with the original code?**

1.	Strong single LED Instantaneous Current:4.9mA.

**2. After commenting out the standard output drive and uncommenting "Weak" drive, how much current does a single LED draw?**

2.	Weak single LED Instantaneous Current:4.89mA.

**3. Is there a meaningful difference in current between the answers for question 1 and 2? Please explain your answer, 
referencing the [Mainboard Schematic](https://www.silabs.com/documents/public/schematic-files/WSTK-Main-BRD4001A-A01-schematic.pdf) and [AEM Accuracy](https://www.silabs.com/documents/login/user-guides/ug279-brd4104a-user-guide.pdf) section of the user's guide where appropriate.**

3.	There is no significant difference in the current consumption in the weak and strong drive strength modes. This can be explained from the reference on page titled **“User Interface”- Main Board Schematic**. There are 3k resistors for each LED. Since there are fixed resistor values; the current that will be drawn from the GPIO pins even under a “strong” drive strength will remain equal to the current drawn by the “Weak” signal strength. The LED0 is present on pin PF4 and LED1 is present on pin PF5.

**4. Using the Energy Profiler with "weak" drive LEDs, what is the average current and energy measured with only LED1 turning on in the main loop?**

4.	Weak Single LED Average Current and Energy – Current:4.69mA ; Energy:11.95uWh.

**5. Using the Energy Profiler with "weak" drive LEDs, what is the average current and energy measured with both LED1 and LED0 turning on in the main loop?**

5.	Weak Double LED Average Current and Energy – Current:4.86mA;Energy:12.25uWh.
