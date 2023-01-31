# Changelog  
  
| modName    | WhimChaser (WHIM) by Axial Aerospace                              |
| ---------- | ----------------------------------------------------------------- |
| license    | GPL-2.0                                                           |
| author     | artwhaley and zer0Kerbal                                          |
| forum      | (https://forum.kerbalspaceprogram.com/index.php?/topic/204900-*/) |
| github     | (https://github.com/zer0Kerbal/zer0Kerbal/WhimChaser)             |
| curseforge | (https://www.curseforge.com/kerbal/ksp-mods/WhimChaser)           |
| spacedock  | (https://spacedock.info/mod/3071)                                 |
| ckan       | WhimChaser                                                        |

## Version 0.5.99.1-prerelease `<On a Wing and a Prayer>` edition

* Released
  * 29 Jan 2023
  * for Kerbal Space Program 1.12.5
  * by [zer0Kerbal](https://github.com/zer0Kerbal)

### Summary

* lots of linting and updates
* IVA
  * now uses mk2CockpitStandardInternals instead of mk1CockpitInternal (2 crew vs 1)
* Compatibility
  * Added
    * <KerbNet.cfg> v1.0.0.0
    * <KerbalInventorySystem.cfg> v1.0.0.0
    * <kOS.cfg> v1.0.0.0
    * <RemoteTech.cfg> v1.0.0.0
    * <TACLS.cfg> v1.0.0.0
      * 2 crew
        * 3 days for both pod and smaller service module
        * 7 days for service module
        * removes some resources from serviced modules to make space for supplies
    * <Ghostparts.cfg> v1.3.0.0
      * will be haunting until full release, then shut off but still included.
  * Updated
    * <OnDemandFuelCells.cfg> v1.1.0.0

### Changes 0.5.99.1

### Parts 0.5.99.1

* <whimChaser.cfg>
  * 'maxTemp' set to 1500, was 3400
  * 'deflectionLiftCoeff' moved into [ModuleLiftingSurface]
  * 'dragCoeff' moved into [ModuleControlSurface]
  * [ModuleReactionWheel]
    * `PitchTorque` = 10 {same}
    * `YawTorque` =  10 {same}
    * `RollTorque` =  5
    * `torqueResponseSpeed` = 10 {commented out}
    * [ElectricCharge] = 0.25 {down from 0.3}
  * [ModuleResourceConverter] from 0.75 to 1.0 `ElectricCharge` consuming 0.001 instead of 0.00075 `MonoPropellant`
  * [ModuleDataTransmitter] stats now equal 16S DIRECT; except still RELAY instead of Direct
  * [ModuleRCSFX]
    * `runningEffectName` now {running} was {runningRCS}
  * `EngineType` = LiquidFuel instead of {LFO}
  * IVA
    * now uses mk2CockpitStandardInternals instead of mk1CockpitInternal (2 crew vs 1)
* closes #7 - IVA interior
* closes #14 - Missing IVA
* closes #17 - part.cfg bugs

### Assets  0.5.99.1

* update textures to DXT5
* Model has no lights, so cannot add to part.cfg
* closes #53 - Asset Updates
* closes #13 - Lights not working

### Compatibility 0.5.99.1

* Add
  * <KerbalInventorySystem.cfg> v1.0.0.0
  * <KerbNet.cfg> v1.0.0.0
  * <kOS.cfg> v1.0.0.0
  * <RemoteTech.cfg> v1.0.0.0
  * <TACLS.cfg> v1.0.0.0
* Fix <OnDemandFuelCells.cfg> v1.0.1.0
  * misplaced @ was O@x
* closes #10 - **kOS**
* closes #11 - **RemoteTech**
* closes #12 - Cargo

### License 0.5.99.1

* Updated License: GPL-2.0
  * was: Expat-MIT
* closes #58 - Update License

### Localization 0.5.99.1

* Create
  * [WhimChaser.cfg] v1.0.0.0
    * adds localized tags to parts
  * Localization/
    * <en-us.cfg> v1.2.0.0
    * [readme.md] v2.1.2.0
    * [quickstart.md] v1.0.1.1
* updates #23 - Localization Master
* closes #24 - Localization - English <en-us.cfg>
* closes #57 - Add localized tags to parts
* closes #55 - Localization

### Documentation  0.5.99.1

* Update all documentation to current standards
* closes #54 - docs/

### Status 0.5.99.1

* Issues
  * closes #59 - WhimChaser (WHIM) 0.5.99.1-prerelease `<On a Wing and a Prayer>` edition
  * closes #60 - 0.5.99.1 Verify Legal Mumbo Jumbo
  * closes #61 - 0.5.99.1 Update Documentation
  * closes #62 - 0.5.99.1 Update Social Media
  * closes #40 - Update AA WhimChaser (end beta - new release)

---

## Version 0.5.99.0-adoption `<Thank you artwhaley>` edition

* Released on 2021-09-17
* For Kerbal Space Program 1.12.2

### `>>-- adopted for curation by zer0Kerbal --<<`

DO A CLEAN INSTALL: DELETE EXISTING THEN RE-INSTALL
Resources and corresponding tanks have changed density/volume/cost/mass

### Parts

* updated
  * part.cfg:
    * added explosionPotential
  * nodes (flipped orientation as needed)

* updates #17 - part.cfg bugs

### Changelog, .version, Readme.md

* created Changelog.cfg [KERBALCHANGELOG] (.this)
* Add license field
* Add author node
* Add version naming field
* added additional fields in .version (might need to tweak urls)
* added shields to Readme.md

### Online

* GitHub Repo
* created Forum Thread
* updated SpaceDock
* updated CKAN/NetKAN

### modernization, polish, update pass on .cfg

* mesh = with MODEL{}
* .tga -> .dds ( 12.0mb -> 2.66mb )
  * <rescuepod4db.mbm> 4.0mb -> 1.33mb
  * <servicemodule.mbm> 4.0mb -> 1.33mb
  * <rescuepod4db.mbm> 4.0mb -> 0mb (eliminated)
* in patches
* deploy/release process

### Adoption by zer0Kerbal

* Adoption Papers
* Adoption Notice
* licenses
  * for existing repo/postings

### Organize for adoption

* folder structure
* Add
  * license(s) file(s)
  * .version file
* automated backend
* jsons
* Changelog.md -> Kerbal Changelog Changelog.cfg
* Updated Readme.md
* changelog into separate file

### Asset Updates

* moved art into .this/Assets/
* updated texture pointers in model (original, png, dds included)
* create Assets/ folder
* convert from mesh to MODEL
* rename
  * models to unique names
  * textures to unique names
* update
  * model pointers (.png et al to .dds)
  * model texture pointers to new names
* relocate assets to Assets/
* eliminate
  * duplicate textures
  * duplicate models
* relocate part.cfg to Parts/

### docs/

* Add
  * [`_config.yml`]
  * [Attribution.md] v1.0.7.1
  * [ManualInstallation.md] v1.1.8.0
  * [404.md] v1.0.3.2
  * [LegalMumboJumbo.md] v1.0.5.1
  * [Localizations.md] v1.1.7.0
  * [Marketing.md] v1.0.1.0
  * [Notices.md] v1.0.1.0
  * [Part-Catalog.md] v1.1.4.1
  * [Why.md] v1.1.0.0
* closes #4 - Needs a wiki

### Localization

* Localization
  * .this/Localization/
  * localization (en-us.cfg)
  * phrasing a smudge
* Create
  * Localization/
    * <en-us.cfg>
    * [readme.md] v2.1.2.0
    * [quickstart.md] v1.0.1.1
* updates #23 - Localization - Master
* closes #24 - Localization - English (United States) <en-us.cfg>
* closes #3 - Localization

### Status 0.5.99.0

* Issues
  * closes #43 - WhimChaser (WHIM) 0.5.99.0-adoption `<Thank you artwhaley>` edition
  * closes #44 - 0.5.99.0 Verify Legal Mumbo Jumbo
  * closes #45 - 0.5.99.0 Update Documentation
  * closes #46 - 0.5.99.0 Update Social Media
  * closes #18 - ***Repo***
  * closes #19 - ***Social***
  * closes #20 - **Legal MumboJumbo**
  * closes #21 - ***Adoption***
  * closes #49- 0.5.0.0-release
  * closes #50- 0.5.5.0-release
  * closes #42 - Previous Archival Releases

---

## Version 0.5.5.0-release

* September 2, 2014

* docking ports 'control from here' feature working

### Status 0.5.5.0

* Issues
  * closes #50- 0.5.5.0-release
  * closes #42 - Previous Archival Releases

---

## Version 0.5.0.0-release - `<Service Module>` edition

* September 2, 2014
* For Kerbal Space Program 0.25

* improved main pod
  * mesh
  * texture
* adds
  * two service modules
    * They're heavy and they don't provide any lift
    * designed to be detached before re-entry!
    * integrated junior compatible docking ports
    * give additional
      * fuel, battery, and monopropellant

### Status 0.5.0.0

* Issues
  * closes #49 - 0.5.0.0-release
  * updates #42 - Previous Archival Releases

---

## Version 0.4.0.0-release

* No changelog provided

---

## Version 0.3.0.0-release

* No changelog provided

---

## Version 0.2.0.0

* Version 2
* For Kerbal Space Program 0.24.2
* Released on 2014-08-27

* improvements to
  * mesh
  * texture
  * Still not finished, by far, but better than they were!
* part.cfg
  * Added
  * remote control/flight without any kerbals onboard...
  * which is useful for rescue missions
  * keeping with the capabilities of the actual Dream Chaser as well!

---

## Version 0.1.0.0

* Version 1
* For Kerbal Space Program 0.24.2
* Released on 2014-08-27

* No changelog provided

---
