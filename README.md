# ChaosAdditionsMaven
## Chaos Awakens
Chaos Awakens is a remaster of both the very iconic mod [OreSpawn](https://www.orespawn.com/download.html) and [SoulsOfTheFallen's Chaos Awakens mod pack](https://web.archive.org/web/20180314164908/http://www.dangerzonegame.net/mods.html), built from the ground up. The branch for the 1.16.5 version for Minecraft Forge is located at the [Chaos Awakens Github](https://github.com/ChaosAwakens/ChaosAwakens).

## Chaos Additions
Chaos Additions is an addon for Chaos Awakens that adds AIOTs and a new material, Sapphire.

## Usage
#### Make sure to NOT select the dependencies and respository that are inside the buildscript.
To use this maven you should put this code into the repository section of your build.gradle

	maven {
		name = "ChaosAdditionsMaven"
		url = "https://raw.github.com/Blackout03/ChaosAdditionsMaven/main"
	}
	maven {
		name = "ChaosMaven"
		url = "https://raw.github.com/ChaosAwakens/ChaosMaven/main"
	}
	maven {
		name = "GeckoLib"
		url "https://dl.cloudsmith.io/public/geckolib3/geckolib/maven/"
	}
    
You must also add this code to the dependencies section of your build.gradle and update the Chaos Additions, the Chaos Awakens and the Geckolib versions to the latest for the current version of Minecraft that Chaos Additions is updated too.

	implementation fg.deobf("com.blackout:chaosadditions:1.16.5-0.3")
	implementation fg.deobf("io.github:ChaosAwakens:1.16.5-0.9.0.3")
	implementation fg.deobf('software.bernie.geckolib:geckolib-forge-1.16.5:3.0.52')
