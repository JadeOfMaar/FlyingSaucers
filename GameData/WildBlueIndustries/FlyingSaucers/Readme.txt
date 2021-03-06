Kerbal Flying Saucers: Build Flying Saucers in KSP!

Have you ever wanted to pretend that your kerbals found a crashed flying saucer and then reverse-engineered it? With Kerbal Flying Saucers (KFS), now you can! KFS is a mod that lets you research and build your own custom flying saucers that work within established gameplay mechanics while providing an exotic twist. It�s as easy as mixing and matching components to create a vehicle suited to your needs. And with its custom tech tree branch you can simulate your reverse-engineering efforts via the stock science system.
Kerbal Flying Saucers supports Pathfinder, MOLE, DeepFreeze, OSE Workshop, KIS/KAS, CTT, Snacks, TAC-LS, and more.

---Real-World References---

Popular Mechanics, November 2000: �America�s Nuclear Flying Saucer� (https://books.google.com/books?id=MxXlKb9wIe0C&lpg=PP1&lr&rview=1&pg=PA66#v=onepage&q&f=false
)
VZ-9 Avrocar: (http://www.nationalmuseum.af.mil/Visit/MuseumExhibits/FactSheets/Display/tabid/509/Article/195801/avro-canada-vz-9av-avrocar.aspx)
Wired: �Declassified at Last: Air Force�s Supersonic Flying Saucer Schematics� (https://www.wired.com/2012/10/the-airforce/)
Northrop NS-97: (https://s-media-cache-ak0.pinimg.com/originals/53/f7/48/53f7489bf06f582eeb1f68a3a42fb2aa.jpg)

---INSTALLATION---

Copy the contents of the mod's GameData directory into your GameData folder.

--RELEASE NOTES---

0.4.3
- Updated FX, icons, plumes, bulkhead profiles, and Flapjack breaking forces- thanks JadeOfMaar!

0.4.2
- Bug fixes

0.4.1
- Recompiled for KSP 1.6

0.4
- Updated to KSP 1.5.X
- Fixed issues with the Kray Kray experiment not working properly.
- The Kray Kray now properly unlocks whole tech tree nodes upon a successful breakthrough research result.

0.3.12
Last release for KSP 1.4.5!

Bug Fixes & Enhancements
- Fixed issue where switching Play Modes would cause some files to not be renamed and cause all kinds of fun for players...
NOTE: For the changes to take effect, you'll need to switch your Play Mode to some mode other than the current one, then switch it to the desired mode.

0.3.11
- Added Large Tail Fin: This is a larger version of the Flapjack's tail fin for use on the Excalibur.

0.3.10
- Added missing parts.
- Added new WBIGraviticLift module. You can control it via the Flight Operations Managar, or via throttle. Example config:

	MODULE
	{
		name = WBIGraviticLift
		ConverterName = Gravitic Lift
		StartActionName = Start Gravitic Lift
		StopActionName = Stop Gravitic Lift
		ToggleActionName = Toggle Gravitic Lift
		FillAmount = 1.0
		AutoShutdown = false
		GeneratesHeat = false
		UseSpecialistBonus = false
		startEffect = effectStart
		stopEffect = effectStop
		runningEffect = effectRunning

		//Maximum acceleration in meters per second per second.
		maxAcceleration = 20

		//EfficiencyBonus is auto-calculated. The more massive the craft, the higher the "bonus," which translates into
		//consuming and producing input/output resources faster.
		//So instead of EfficiencyBonus, we use specific impulse to determine how well we use the resources.
		//Math: acceleration * total vessel mass = lift force.
		//EfficiencyBonus = lift force / (9.81 * specificImpulse).
		//Resources are consumed & produced at Ratio * EfficiencyBonus.
		specificImpulse = 1
		 
		//...or liquid fuel, or whatever...
		INPUT_RESOURCE
		{
			ResourceName = Graviolium
			Ratio = 0.0016875
			FlowMode = STAGE_PRIORITY_FLOW
		}
		OUTPUT_RESOURCE
		{
			ResourceName = StaticCharge
			Ratio = 0.05
			DumpExcess = false
		}
	}

0.3.9

Excalibur (WORK IN PROGRESS!)
- Added Large Body Flap. It works the same way as the Flapjack's body flap.
- Added S-4 "Excalibur" Cockpit prototype.
- Finished modeling and unwrap of the storage sections and engineering core- texturing to follow.
- Removed Double Outer Section.
- Updated wording on node switching for the Inner Section, and added visual cues to help identify configuration for the outer sections.
- Added particle effects to the engineering core.

Bug Fixes & Enhancements
- Fixed Crazy Mode controls vanishing when a vessel without a gravitic engine is loaded into scene.
- Fixed NRE produced by converters when BARIS isn't installed.
- Fixed issue preventing multiple saucers within physics range of each other from hovering at the same time.
- Fixed issue where craft wouldn't hover on airless bodies.
- Graviolium won't be stripped from your vessels upon launching from the VAB/SPH if you're in Sandbox or Science mode.
- Crazy Mode can now be used when the craft is considered to be sub-orbital as well as when it is flying.

0.3.8
- Fixes Play Mode failing to rename certain files. NOTE: You might need to reset your current play mode. Simply open the WBT app from the Space Center, choose another mode, press OK, and again open the app, selecting your original play mode. Then be sure to restart KSP.

0.3.7
- Fix for Stardust not collecting Graviolium.

0.3.5
- Minor update to the Hydroscoop to use the new WBIResourceHarvester.

0.3.4
- WBT update.
- Fixed click-through issues with windows displayed in the editor.

0.3.3
- Added experiment lab to MPL and experiment container to the Science Box.
- Bug fixes for experiments.

0.3.2
- WildBlueTools update.

0.3.1
- Updated part symmetry axis. Thanks for the investigation, Vardicd & shdwlrd! :)
- You can now set the gravitic engine's forward, reverse, and VTOL thrust modes through action groups.
- You can now toggle Crazy Mode on and off through action groups. NOTE: this only works in the forward direction.
- Added new sounds to the Excalibur Engineering Core's generators.
- The Excalibur Inner Section now has node toggles to make it easier to switch between adding two standard-sized outer sections, or one standard outer section and two half-sections.
- Made a better sound loop for the gravitic engine.
- More infrastructure work done on KerbalActuators for kOS support.
- Updated a couple of part tool tips for clarity.
- Re-added IVA props that I missed during latest MAS integration.
- Fixed mesh gaps as best as possible for Excalibur's template parts and adjusted the shape to better fit 2.5m tall payloads.
- Fixed top node placement on the fusion reactor.
- Fix for multiple part tool tips appearing when you attach new parts. Hopefully this will solve it once and for all!

0.3.0
- Flapjack IVA upgraded courtesy of MOARdv :) NOTE: You'll need MOARdv Avionics Systems 0.20.1 or later.
- Added new S-4 Excalibur parts category.
- Added test parts for the S-4 Excalibur mothership. THESE ARE SUBJECT TO CHANGE WITHOUT NOTICE.

0.2.11
- Un-broke the template managers.
- Finally straightened out the Half Keel to have the proper model and colliders.

0.2.10
- Fixed missing collider on the Half Keel.
- The Gravitic Engine won't kill the throttle if you turn off Hover Mode and have forward thrust set during flight. This should make it easier to transition from VTOL to forward flight.

0.2.9
- Added A-51 Half Keel for those times when only half a saucer will suffice.
- Recompiled for KSP 1.4.4

0.2.8
- Fixed issues where the Flapjack docking port and Gravitic Engine's RCS thrusters wouldn't work with the cargo bay attached. Thanks for the solution, MOARdv! :)

0.2.7
- Fixed issue where the throttle wouldn't be updated during Hover Mode and forward flight.

0.2.6
- Fixed issue where the gravitic engine wouldn't produce acceleration when MechJeb tried to execute a maneuver node.
- Added infrastructure to KerbalActuators to support MOARdV Avionics Systems.
- Removed debug code left over from last release.
- Improved Crazy Mode performance when there are no other vessels in physics range.

0.2.5
- In the flight scene, you now have the ability to recovery resources that are normally stored in the Refinery.
- Some resources, like Graviolium, are now considered restricted in OmniStorage tanks. You can allocate space for a restricted resource in the VAB/SPH, but it won't be added to the container until launch. This avoids the problems associated with adding resources in the editor that can give a craft a negative part cost. No such restriction applies to vessels reconfigured after launch.
- Lowered the Flapjack cargo bay floor slightly to make it easier to sit kerbals inside using the external command seat.
- Crazy Mode movement is now affected by thrust limit in addition to throttle setting.
- Fixed issue with Crazy Mode failing to function when multiple vessels are loaded in physics range.

0.2.4
- The gravitic engine now consumes GravityWaves while in Hover Mode.
- The gravitic engine now has a built-in Terrain Awareness and Warning System (TAWS) for Crazy Mode. TAWS will halt the craft if using Crazy Mode will result in a crash.
- GravityWaves produced in the gravitic generator will fade away if the generator is turned off. They weren't intended to stick around indefinitely...
- Fixed missing tech tree node icons.
- Fixed issue where resources were consumed while reconfiguring a disassembled part.

0.2.3
- Gravitic engine acceleration now relies on accelerationCurve, which is tied to the throttle setting and thrust limiter. The accelerationCurve will likely need performance tuning...
- Fixed symmetry issues with Flapjack saucer sections.
- Fixed issue where acceleration could be applied even when the gravitic engine wasn't running.
- Fixed NREs generated when a saucer crashes.
- Fixed FX warnings generated when a saucer crashes.
- Fixed OmniStorage not remembering its storage configuration. NOTE: You might need to redo your omni storage containers.
- Fixed OmniStorge issue with KIS volume configuration.

0.2.2
- NRE fixes for turning on/off converters when BARIS isn't installed.
- Fixed missing IntakeLqd on the Hydroscoop.
- Removed RPM dependency - Thanks to MOARdv for updating MAS to support the ASET Avionics HUD!
  NOTE: You'll need MAS 0.16.0.

0.2.1
- Improved the gravitic engine's ability to propel asymmetric craft designs. Aero forces still apply.
- Gravitic engine now bases "forward" on the vessel control point. As an example, forward could be respective to a cockpit or a docking port. VTOL lift is unaffected.
- Excluded experiments from KEI.
- Potentially excluded experiments from [x]Science! Needs testing...
- Fixed issue with tool tip window appearing multiple times.
- Added additional tool tips.

0.2.0 Initial Alpha Pre-Release

---ACKNOWLEDGEMENTS---
Icons made by Freepik from www.flaticon.com

---LICENSE---
Art Assets, including .mu, .mbm, and .dds files are copyright 2017 by Michael Billard, All Rights Reserved.

Wild Blue Industries is trademarked by Michael Billard. All rights reserved.
Note that Wild Blue Industries is a ficticious entity 
created for entertainment purposes. It is in no way meant to represent a real entity.
Any similarity to a real entity is purely coincidental.

Source code copyright 2017 by Michael Billard (Angel-125)

    This source code is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.