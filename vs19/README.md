# Compilation instructions for VS19

Before compiling this program in Visual Studio 2019, you first need to extract the libraries librtlsdr and libusb into two folders "librtlsdr" and "libusb" parallel to the rtl_433_win folder.

Regarding librtlsdr, use the repository https://github.com/winterrace/librtlsdr which adds build files for Visual Studio.

Regarding libusb, use a release build (e.g. libusb-1.0.23.7z) from the official repository https://github.com/libusb/libusb. 

The folder structure has to look like this

    rtl_433_win
        include
        src
        vs19
        <and so on>
    
    librtlsdr
        include
        src
        vs19
        <and so on>
        
    libusb
        include
        MS32
        MS64
        <and so on>
        
        
For librtlsdr Follow the compilation instructions for x64 or Win32.
    
Then simply open rtl_433_win/vs19/rtl_433.sln in Visual Studio and select between x64/Win32 and debug/release build options.
