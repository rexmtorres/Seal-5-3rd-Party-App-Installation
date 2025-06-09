# BYD Seal 5 3rd-Party App Installation
Instructions on how to install non-market apps on your BYD Seal 5 DM-i system.  

<details>
  <summary>DISCLAIMER</summary>
  
  ### WEBSITE DISCLAIMER
  The information provided by Rex Mag-uyon Torres ("we," "us," or "our") on https://github.com/rexmtorres/seal-5-3rd-party-app-installation (the "Site") is for general informational purposes only. All information on the Site is provided in good faith, however we make no representation or warranty of any kind, express or implied, regarding the accuracy, adequacy, validity, reliability, availability, or completeness of any information on the Site. UNDER NO CIRCUMSTANCE SHALL WE HAVE ANY LIABILITY TO YOU FOR ANY LOSS OR DAMAGE OF ANY KIND INCURRED AS A RESULT OF THE USE OF THE SITE OR RELIANCE ON ANY INFORMATION PROVIDED ON THE SITE. YOUR USE OF THE SITE AND YOUR RELIANCE ON ANY INFORMATION ON THE SITE IS SOLELY AT YOUR OWN RISK.

  ### EXTERNAL LINKS DISCLAIMER
  The Site may contain (or you may be sent through the Site) links to other websites or content belonging to or originating from third parties or links to websites and features in banners or other advertising. Such external links are not investigated, monitored, or checked for accuracy, adequacy, validity, reliability, availability, or completeness by us. WE DO NOT WARRANT, ENDORSE, GUARANTEE, OR ASSUME RESPONSIBILITY FOR THE ACCURACY OR RELIABILITY OF ANY INFORMATION OFFERED BY THIRD-PARTY WEBSITES LINKED THROUGH THE SITE OR ANY WEBSITE OR FEATURE LINKED IN ANY BANNER OR OTHER ADVERTISING. WE WILL NOT BE A PARTY TO OR IN ANY WAY BE RESPONSIBLE FOR MONITORING ANY TRANSACTION BETWEEN YOU AND THIRD-PARTY PROVIDERS OF PRODUCTS OR SERVICES.
</details>

&nbsp;

## Preface

Apart from installing apps through the BYD app marketplace, which offers an **extemely** limited (for now) set of apps, there are 2 unofficial ways of installing 3rd-party apps, which I will show you in this tutorial.  The 2 methods that will be shown here are, generally speaking, safe to follow.  However, as they are ***unofficial*** methods, they might affect your warranty.  So, follow at your own risk.  I take no responsibility, whatsoever, for any loss or damage incurred as a result of using and relying on the information on this tutorial.

Please also note that, depending on your infotainment system version, the steps mentioned here, to install apps, may or may not work.

&nbsp;

## Method 1: Sideloading w/out an unlocked package manager

1. Prepare a USB flashdrive by formatting it to **FAT32** on a (Windows/Mac/Linux) computer.  Note that, especially when using Windows' built-in formatter, the FAT32 option may not appear if your flashdrive's capacity is greater than 32GB.  So you may want to use a smaller capacity flashdrive.

2. In your FAT32-formatted flashdrive, create a folder named "Third Party Apps 63" (without the quotes).
   
   *Note: This is specifically for the Philippine market.  If you're outside the Philippnes, replace "63" with your respective [country code](https://countrycode.org/philippines).*
   
   ![Third Party Apps 63](./screenshots/Screenshot%202025-06-07-133147.png)

3. Copy your downloaded APKs into the "Third Party Apps 63" folder.
   
   *Note: Be sure that you trust the source of your APKs.  One of the more popular sources of APKs is [APKPure](https://apkpure.com/).  Also note that APKPure provides 2 formats of an application package: APK and APKX.  Be sure to choose APK.  APKX is APKPure's own extension of the APK format and you will need an additional application manager to install it.*

4. Eject your flashdrive from your computer.

5. With your BYD Seal 5 off, plug your flashdrive into the USB data port (lower USB port) located underneath the center console.

6. Start your car and wait for the infotainment to initialize.

7. Once the system has initialized, you will be prompted to enter a password.  Enter "BYD6125F" (without quotes) and press OK.

   ![password](./screenshots/20250607_091221.png)

8. You will then be able to see the list of the APKs you copied.  Tick the checkbox on the APKs you want to install and press Install. The "Success" counter at the bottom-right corner will indicate the number of apps successfully installed, while the "Failed" counter will indicate those that didn't install.  Failed installation can either mean that the APK you downloaded is corrupted, or that the BYD system does not support them.

   ![apks](./screenshots/20250607_091346.png)

9. After installing them, you can press Back or Home on the navigation bar and you should see the icon/s of the app/s you installed.

### Note:
With this method, you will need to manually download the APK files of the apps you want to to update/install.  You will then have to perform steps 3-8 every time you want to apply the updates or install additional apps.

&nbsp;

## Method 2: Using the unlocked package manager

1. If you haven't done so already, follow steps 1 and 2 in [Method 1](#method-1-sideloading).

2. Download [CX File Explorer](https://apkpure.com/search?q=cx+file+explorer) and copy the APK to the "Third Party Apps 63" folder.

3. Download the [unlocked package manager](https://workupload.com/file/EgYhyaba92E).  Unzip it and copy "PackageInstallerUnlocked.apk" into the "Third Party Apps 63" folder.

4. Install **CX File Explorer** (***only***) by following steps 5-8 in [Method 1](#method-1-sideloading).

   ***Warning: Do not yet install the unlocked package manager (PackageInstallerUnlocked.apk) at this point!***

5. Launch **CX File Explorer**.  Grant the necessary permissions it may ask.

6. Click the "Apps" section.
   
   ![CX File Explorer - Apps](./screenshots/20250607_093005.png)

7. Go to the "All" tab.  Find "Package installer" and tick the checkbox to its right.  Then, click "Backup".

   ![CX File Explorer - Backup](./screenshots/20250607_093050.png)

   This will save a copy of your original (locked) package installer in `Main storage -> backups -> apps`.  Please save a copy of this in a safe location (e.g. your thumbdrive or cloud drive).  You may need this to revert the package manager.

   ![Locked package installer backup](./screenshots/20250607_093118.png)

8. Install the unlocked package manager (PackageInstallerUnlocked.apk) you downloaded in step 3 by following steps 5-8 in [Method 1](#method-1-sideloading).

   At this point, you should now be able to install any supported APK by just downloading them anywhere in your infotainment and clicking on the APK file.  You can even install 3rd-party app markets, like [Aurora](https://apkpure.com/aurora-store/com.aurora.store) or the [APKPure](https://apkpure.com/search?q=apkpure) app or [F-Droid](https://f-droid.org/en/), and install additional apps through them.

&nbsp;

# Bonus: microG Installation

The [microG project](https://microg.org/) provides an open-source re-implementation of Google’s proprietary Android user space apps and libraries.  This allows you to install and run apps (e.g. Netflix, Waze) that rely on Google's services, that may otherwise not work without these Google services.  However, not all apps will run even with microG installed.

Depending on which method you choose for installation, download and install **microG Services**, **microG Companion** and **Services Framework Proxy** found here: https://microg.org/download.html

![microG files](./screenshots/Screenshot%202025-06-09%20184928.png)