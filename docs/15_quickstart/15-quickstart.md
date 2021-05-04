﻿# NMRium Quick Start Guide

## 1. Open the program
Open NMRium with the following link:
[https://cdn.nmrium.org/](https://cdn.nmrium.org/)

## 2. Open spectra
To open spectra, your data must be in one of the following file types:

-   Jcamp DX (.dx, .jdx, .jcamp)
-   zipped folder in Bruker format (raw data od processed)
-   Jeol (.jdf)
-   NMRium file (.nmrium)

Drag the file you want to open into the gray box **Drag and drop here** in the middle of the screen. You can open a set of spectra of a molecule by either dragging the spectra individually into the workspace or by dragging a zip folder containing all spectra. Also, you can open several spectra at once in the Bruker folder structure as a zip file.

![](./img/01.png)

## 3. Select a spectrum
On the right side of the workspace, various areas are available in an expandable menu. Click on the head of the **Spectra** field. The measured nuclei (e.g. 1H, 13C, etc) are displayed in the opened field. Click on a nucleus to find the experiments associated with it. To select an experiment, click the corresponding line. The experiment appears in the workspace.

![](./img/02.png)

#### Note on wobble-curves:

If your imported Bruker folder contains so-called **wobble curves**, it is useful to delete them from the list for further processing. You can identify them by the name **wobble**. Click the corresponding spectrum with the right mouse button. In the appearing menu, click **delete** to delete the wobble curve.

#### Note on changing the color of a spectrum:

You can change the color of the spectrum by clicking the colored square in the line for the spectrum. In the appearing window, you can select a different color. For 2D experiments, the colors for the negative and positive cross-peaks are additionally selectable.

4.  ### Delete a spectrum
    

To delete a single spectrum, right-click the spectrum in the menu **spectra** on the right side. Click **delete** in the appearing menu to delete the spectrum. To delete all spectra, click on the trash icon on the left above the listed spectra.

5.  ### Zoom a section
    

To zoom a section of a spectrum, drag over it with the left mouse button. You can repeat this process as often as you like. Double-click anywhere in the spectrum to undo the last magnification step. This step can also be repeated. The intensity level of the signals can be changed using the mouse wheel. To return to the full spectrum, click on the **Zoom-Out** button in the menu bar on the left side of the spectrum.

6.  ### Insert a molecular structure
    

There are two possibilities to insert a molecular structure into the program:

a)  Molfile: Drag the molfile into the workspace. The **Structures** field appears, showing the inserted molecular structure as well as the molecular weight and the molecular formula.

b)  Integrated structure editor: Click on the **Structures** menu on the right side of the screen and then on the **+** sign. A window opens where you can draw your molecular structure. Then click on the **Save** button. In the **Structures** field, the drawn molecular structure appears as well as the molecular weight and the molecular formula.

![](https://lh5.googleusercontent.com/XpsxF0oMjcgqUi0klK_IsGwG3RPaYv5wHw_sC-ruDDYVjza4xu8B1Sjs7NQPKNvcHwS3aMINwKf4ed5bGHiroJYOEjGGbThamJoF_TxK8cuTBS-UxbCp5bd63G_ICgouAinKKDqj)

7.  ### Processing of raw data (currently only 1D)
    

NMRium offers the possibility to perform a Fourier transformation (FT) on the raw data of one-dimensional NMR spectra. To process an FID, open the FID by dragging it into the **Drag and drop here** box (Chapter 2).

![](https://lh4.googleusercontent.com/NGA5uHpt6TofoKE4-IuxuTL4n06a__hJX5TC0KlWn6EiQCYyhfJQhy_RV4uGgbGaSM-1kSctFaisNi36T6RcXJFcONXlfGnH2tpp7-2jt_bSA3F9RX_DhmztNJSQu7TBU7GYxdO3)

1.  Fourier transformation: To prepare the FID for the Fourier transformation, click the **Zero Filling** icon to the left of the spectrum. Set the desired values for **Size** (zero filling) and **Line Broadening** (exponential window function) and click **Apply**. Then start the Fourier transformation by clicking on the **FFT Filter** button to the left of the spectrum.  
      
    Note on values:
    

If you are not sure which values to set, you can use the following recommendations as a reference:

**Size**: Choose twice as many points as in the original FID.

**Line Broadening (LB)**: Specify 0.3 Hz for 1H spectra and 1-3 Hz for 13C.  
  

2.  Phase correction: Click the **Phase correction** icon to the left of the spectrum. You can choose between manual and automatic phase correction.
    

Automatic phase correction: Click the **Apply** button, the phase will be corrected automatically.

Manual phase correction: You can perform zero-order and first-order phase correction.

For zero-order phase correction, click and hold the green **PH0** button above the spectrum. By moving the mouse to the left or right, you can perform phase correction until the signal is correctly phased and release the button. By double-clicking, you can move the pivot point (red line) for the first-order phase correction.

The first order phase correction is performed analogously by pressing **PH1**. The focus should be on the signals that are as far away as possible from the signal under the pivot point. Clicking the **Apply** button completes the phase correction.

  

8.  ### Referencing
    

Click the **Peaks Picking** button to the left of the spectrum. Find your solvent signal (or the reference signal). When you point at it with the crosshairs, press the shift key and the left mouse button at the same time. The value of the signal will be shown both in the spectrum and in a list on the right side of the spectrum in the **Peaks** field. Select one of the two displayed values (in the spectrum single click with the left mouse button, in the list double click with the left mouse button) and enter the correct reference value.

![](https://lh3.googleusercontent.com/PXgE3Ac9L3HPp45sCRVlAazdr8BTX9rM05UdX93e5sIFcVz3UJuHySJ23aLe3kOElzMcXuRPkLN8EBpKJeiI6EMeDg-FO2ILdaEOqPe8sFvbKl79gCRxvELM1_gmtgHkr2FDbp9z)

9.  ### Peak Picking
    

Click on the **Peaks Picking** button. You can choose between automatic peak picking and manual peak picking.

1.  Automatic peak picking: A list appears above the spectrum in which you can specify the maximum number of peaks, the noise factor and the minimum-maximum ratio (Min Max Ratio). Then press **Apply**. The chemical shift of the peaks is displayed both in the spectrum and in a list on the right side of the spectrum in the **Peaks** field.
    
2.  Manual peak picking: Locate a signal. When you see it in the crosshairs, press the shift key and simultaneously the left mouse button. The value of the signal will be shown in a list both in the spectrum and on the right side of the spectrum in the **Peaks** field.
    

  

10.  ### Delete peaks
    

If you want to delete a single peak, find the corresponding signal on the right side of the spectrum in the list in the **Peaks** field. Click the trash icon on the far right of the line, the peak will be deleted.

If you want to delete all peaks, click on the trash icon located above the signal list under the **Peaks** field. Confirm that you want to delete all peaks by clicking **Yes** in the window that opens.

  

11.  ### Choosing the values to display in the "Peaks" list
    

You can display various information in the **Peaks** list. Open the **Peaks** list on the right side of the spectrum. Click on the gear wheel at the top right. All measured nuclei will be displayed. You can choose to display the following values for each nucleus:

-   Peak Number
    
-   Peak Index
    
-   Chemical shift (ppm)
    
-   Chemical shift (Hz)
    
-   Width
    
-   Intensity
    

Place a checkmark next to the values that you want to have displayed for the respective nucleus. Then click on the green check mark at the top right.

12.  ### Integration
    

Click the **Integral tool** button on the left side of the spectrum. To integrate a signal, hold down the Shift key and move the mouse over the signal while holding down the left mouse button. Then release both the Shift and the left mouse button. Proceed in this way with each signal that you want to integrate. The integrals are displayed in a list on the right side of the spectrum in the **Integrals** button.

It is predefined that the relative number of all integrated H atoms is 100. To change the number, click on the sum symbol above the list. In the window that opens, you can either enter the number of H atoms manually and then click on **Set** or accept the number of H atoms specified by the sum formula by clicking on **Set** in the lower area.

  

![](https://lh5.googleusercontent.com/rITtr4tFv7x_OrpEDsa38okP8fkmHcAHxAYO4f7Wqp-6ZM_crH_bT_nNCittjg7YJXzJLUR4oM8JpzydWAM-4b4xA9QdQyRea8yQ4vb5cZIA7Dz4N3hV-1jVmchY6kJ_IUN-tDYY)

  

13.  ### Delete integrals
    

If you want to delete a single integral, find the corresponding signal on the right side of the spectrum in the list in the **Integrals** field. Click the trash icon on the far right of the line, the integral will be deleted. Alternatively, you can click on the red fieldat the bottom of the spectrum that belongs to the respective integral. The corresponding integral will be deleted.

If you want to delete all integrals, click on the trash icon located above the signal list in the **Integrals** button. Confirm that you want to delete all integrals by clicking **Yes** in the appearing window.

  

14.  ### Picking ranges and determination of coupling constants
    

Click on the **Ranges Picking** button on the left side of the spectrum to specify signal assignment ranges, for example to determine coupling constants. You have the option of either manually or automatically defining the assignment ranges:

1.  Automatic ranges picking: A list appears above the spectrum. Click on the button **Auto ranges picking**, the assignment ranges will be determined automatically and displayed both in the spectrum and in a list on the right side of the spectrum in the **Ranges** field. The corresponding coupling constants are determined automatically.
    
2.  Manual ranges picking: Press the Shift key and move the mouse over the range you want to set. The marked assignment range is displayed both in the spectrum and in a list on the right side of the spectrum in the **Ranges** field. The corresponding coupling constants are determined automatically.
    

  

![](https://lh5.googleusercontent.com/uTcr8S37Gb7VSGmoxv9p6tZBRYbj_wd7U81_Kkbhd5EULUpXIAv4EvQWWe5xm2EwkUnVkxPneED3cydPiUIsbV76yzo81xf_NbEyYGFJcK-5AKcqgZbMc-TW9HXqZGWV4oKGPyP8)

15.  ### Delete ranges
    

If you want to delete a single range, find the corresponding range on the right side of the spectrum in the list in the **Ranges** field. Click the trash icon on the far right of the line, the range will be deleted.

If you want to delete all ranges, click on the trash icon located above the signal list in the **ranges** field. Confirm that you want to delete all ranges by clicking **Yes** in the window that opens.

16.  ### Assignment of signals
    

To assign signals, you have to define assignment ranges (Chapter 14) and insert a molecular structure (Chapter 6). Open the **Ranges** and **Structures** fields on the right side. Specify the correct number of relative H atoms by clicking the sum icon above the **Ranges** list. In the window that opens, you can either enter the number of H atoms manually and then click on **Set** or accept the number of H atoms specified by the sum formula by clicking on **Set** in the lower area.

In the list, click the box under the link icon in the line of the signal you want to assign, . A red zero appears there. Then assign the signal by clicking on the corresponding atoms in the structural formula. Proceed in the same way with all other ranges. You can also assign several, different H atoms to a range by clicking successively on all H atoms in the structural formula that belong to the respective signal. If you want to assign diastereotopic H atoms, hold the Shift key while clicking the corresponding H atom in the structure. This makes both diastereotopic H atoms visible.

![](https://lh6.googleusercontent.com/VhRVWcsRgxC-ixsn1kGUzQ1E-x1eI4C5wleAa7yj6uoWjzTgMaqHNIz8mL95F6HunVhkE3-zTwissZs2g_74tDR4W2Bo-QVr7FC0HyYq0BDApXd0PX69lLZlFAnfJG1PDpA5zaK6)

17.  ### Export of assigned spectra
    

To export the assigned spectra, click on the **Export** button to the left side of the spectrum. A field will open where you can select in which format you want to export your spectrum. You have the following options:

-   Export as SVG
    
-   Export as PNG
    
-   Save data
    
-   Copy image to Clipboard
    

Click on **Save data** to save the assigned spectrum with all stored information and to be able to edit it later. An nmrium file is created and offered for download.

#### Note:

A nmrium file is a compressed text file containing all information of the (partially) assigned stored spectra. Depending on the number of spectra contained, saving can take longer, as can opening an nmrium file again.