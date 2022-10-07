# Reported Known Issues

!!! error STOP - Read this first
 Please try and remove all other mods/liveries from the community folder and test our add-on again. This will help rule out conflicts.

    *Most reported issues are caused by conflicts with other mods and liveries. If this does not resolve your issue please continue below.*
!!! danger NO SUPPORT will be provided for unofficial versions of the 787-10 for Microsoft Flight Simulator.
!!! danger No Support for Experimental - use at own risk


# Known Issues

<!-- TEMPLATE DO NOT DELETE 

!!! warning Issue/Bug: Name

    !!! tip *Affected Versions: e.g. Stable, Development*
    
    Issue/Bug Description

    Root Cause 

    !!! Possible Solution or Workaround
    - Solution/Workaround description 

-->

!!! bug NAVRAD frequencies sometimes not entered automatically

    !!! tip *Affected Versions: Development, Stable, Experimental*

    When the user selects an approach on the DEP/ARR page, sometimes the ILS frequency is not automatically set
        
    - The cause of this is under investigation

    !!! Possible Solution or Workaround
        - It is good practice to always check the approach frequencies are set prior to descent.


!!! bug Radio Panels are inop on initial load

    !!! tip *Affected Versions: Development*
    
    
    B78XH Radio Navigation Panels are black or inop on initial load:
    - The root cause of this is under investigation.

    !!! Possible Solution or Workaround
        - Whilst we work on finding a solution, if this occurs, restart the flight before continuing.


!!! bug Authothrottle Disconnect

    !!! tip ""
         *Affected Versions: Development, Stable*

    The Autothrottle stops automatic function, and only listens to user inputs

    -  The root cause of this is under investigation.

    !!! Possible Solution or Workaround
        - Push forward on the yoke until the AT reconnects. 


!!! warning Issue: Toolbar Pushback Addon Issues

    !!! tip *Affected Versions: Stable, Development, Experimental*

    - This 3rd party addon may cause the following issues:
        - Stuck Aircraft
        - Unable to taxi
        - Performance Degradation

    !!! Possible Solution or Workaround
    - Remove the addon from your community folder or wait for developer to update or see next item.
        - Keep the addon but remove it from the toolbar once you have pushed back


!!! warning Issue: Screens are black or inop on initial load

    !!! tip *Affected Versions: Stable, Development, Experimental*
    
    
    B78XH screens are black or inop on initial load:

    - Some 3rd party liveries or texture mods are breaking the state of our custom instruments. **Please do not install addons that modify the `panel.cfg` in the official Packages Directory**

    !!! Possible Solution or Workaround
        - Remove the `panel.cfg` file from any 787-10 livery folder or texture mod.


!!! warning Issue: Center Fuel Pump Switches Cause APU Disconnect

    !!! tip ""
        *Affected Versions: Development, Stable, Experimental*

    Toggling the center fuel pump switches to ON causes APU shutoff

    -  The root cause of this is under investigation. It affects the default 787 as well.

    !!! Possible Solution or Workaround
        - Do not toggle center fuel pumps until both engines are running.


!!! warning Issue: 180th Meridian Visual Bug

    !!! tip *Affected Versions: Development, Stable, Experimental*
    Due to the way the world is generated, the flight plan seems to "end" and wrap back around the Earth in a horizontal line when crossing the 180th meridian.

        The ND is rendered as "square" with coordinates... the left side of the square is 180W and right side is 180E
       


    !!! Possible Solution or Workaround
        - This is simply a visual bug and is the default behavior of all MSFS aircraft. **The flight plan will continue as normal past the 180th meridian**


## Common MSFS Issues Impacting All Aircraft

!!! warning bug "MSFS Performance Degradation In-Flight"
    ### MSFS Performance Degradation In-Flight

    !!! tip ""
        *Affected versions: Stable, Development*

    Reports in the MSFS forums detail issues impacting FPS performance in the sim. Notably this occurs during flights that are longer than 2 hours but is not contained to this metric. You may see your normal FPS drop to <10 FPS as a result of this issue.


    Follow the MSFS Forums Discussion - [here](https://forums.flightsimulator.com/t/after-playing-a-few-hours-fps-drops-from-40-to-5fps/389603/941).

!!! warning CTD (Crash to Desktop)
    

    !!! tip "" 
        *Affected versions: Stable, Development*

    With the current state of the sim it is basically impossible to analyze CTDs let alone fix them as MSFS does not provide any tools or logs for analyzing CTDs.

    If we can reliably reproduce a CTD in our aircraft we will try to fix it or at least work around it. But most CTDs are very unpredictable and can be caused by many things:

    - Add-ons and mods
        - Liveries<br/>(flightsim.to just removed 1000s of them because of that)
        - Airports
        - Basically any add-on and mod that may be outdated or have conflicting files
    - MSFS itself (e.g. Rolling Cache is often a cause)
    - Hardware (GFX Card and Driver, Overclocking, etc.)
    - Controllers and Drivers
    - Any third party application that connects to MSFS

    Unfortunately just using the sim's API functions might trigger a CTD, so the trigger could be the aircraft but the root cause would be the sim.

    If you can reproduce it reliably please share this information with us on Discord or our GitHub so we can try to also reproduce it. This would be the first step to fix anything.

    Root Cause

    Various possible reasons - impossible to determine at the moment.

    !!! note ""
        Possible Solution or Workaround

    There also is currently no known guaranteed solution, however users have found success with by trying the following:

    1. Remove everything from the Community folder - **really everything**!
    2. Perform a [Clean Install](../installation.md#clean-install-steps)
    3. Stop any third party application which connect to MSFS<br/>
       FSUIPC, YourControls, Fs2Crew, SPAD.next, ...
    4. Run without live weather and/or live traffic.
    5. Delete your rolling cache in the sim and create a new one.
    6. Delete any manual cache in the sim and create new ones.
    7. Run the game as Administrator.
    8. Visit and read the [MSFS Known Issues Page](https://flightsimulator.zendesk.com/hc/en-us/articles/360016027399-KNOWN-ISSUES-Last-update-July-28-2021-) OR [MSFS Troubleshooting & Support](https://flightsimulator.zendesk.com/hc/en-us/sections/360004475200-Troubleshooting-Support-Windows-10-PC)

    ^^Additional Information^^

    Please also search in the MSFS Discord and Forum for CTD causes and solutions.

    [MSFS ZenDesk Safe-Mode-FAQ](https://flightsimulator.zendesk.com/hc/en-us/articles/4405893759378-PC-versions-Safe-Mode-FAQ){target=new}

    [MSFS ZenDesk CTDs-issues-Basic-Troubleshooting](https://flightsimulator.zendesk.com/hc/en-us/articles/4406280399250-All-versions-Crashing-CTDs-issues-Basic-Troubleshooting){target=new}

    [MSFS ZenDesk CTDs-issues-Advanced-Troubleshooting](https://flightsimulator.zendesk.com/hc/en-us/articles/4406280653202-All-versions-Crashing-CTDs-issues-Advanced-Troubleshooting){target=new}

    [MSFS Forum ctd-analysis-by-community](https://forums.flightsimulator.com/t/kadw-andrews-ctd-analysis-by-community-contributions/465405){target=new}

    !!! info "Peripherals"
        This is an important snippet from MSFS known issues.

        If you are getting CTDs, it could be one of your peripherals disconnecting sometime during the flight, which then causes the sim to CTD.

        It could be anything from a usb drive to a controller. Please try to minimise how many peripherals you have connected.
