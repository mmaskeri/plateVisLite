# plateVisLite
Generate ChemDraw CDXML colormap for up to 12x8 well screening data, inspired by plateVis (Maskeri 2018)

plateVisLite offloads linear interpolation and colormapping to Excel's built-in Conditional Formatting function to provide quick and easy colormapping of up to 12x8 wells worth of data. CDXML data for ChemDraw is generated by a set of macros and assembled into cell E20; the cell can then be copied and pasted (directly, ChemDraw 17 or later, or as CDXML text). Appropriately-spaced axes are provided as well in cell E23 and can be easily aligned to the colormap for a professional appearance.

In theory, the code can be expanded easily beyond 12x8 wells, but this requires breaking apart the resulting CDXML text (Excel cells can only hold up to 32,767 characters). For ease of use--namely to fit the requisite data in a single Excel cell--the CDXML representation has been stripped of non-essential data, which is interpolated by ChemDraw to create a full representation.

Please consider acknowledging plateVisLite in publications for which it is used to generate graphics:

plateVisLite, Maskeri, M. A., 2021, <github.com/mmaskeri>

Example default colormap (aligned with provided axes):

![image](https://user-images.githubusercontent.com/11822744/120084770-9efee900-c098-11eb-8e4f-578953e0867e.png)
