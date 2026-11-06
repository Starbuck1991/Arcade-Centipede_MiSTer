# Cabinet lamp outputs

Cabinet lamp adaptation by J. M. Artés (2026). All original core authors, copyright notices and licenses are retained. This is a small integration with the original arcade hardware logic, not a replacement for that work.

Exposes the active-low original coin-counter latch lamp outputs; synchronizes them to the MiSTer clock. Millipede is outside this change. The game firmware retains control of the lamp sequence and blinking: no extra credit counter or blink timer is introduced.

The outputs use the standard MiSTer keyboard LED interface: player 1 lamp on Num Lock, player 2 lamp on Caps Lock. The custom Main configuration can restrict delivery to the selected I-PAC; this core does not program the controller.

Use releases/Centipede_Leds.rbf and set the matching MRA rbf element to Centipede_Leds. Preserve the ROM layout of this core revision. Original ROMs are not included. The original Quartus project remains buildable; sys/pll_q19.qip references the existing PLL IP when compiling with Quartus 19.1.

Validation: Compiled and installed; individual physical validation is not recorded.
