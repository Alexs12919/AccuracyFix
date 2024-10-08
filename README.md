<h1 align="center">Counter-Strike 1.6 Accuracy Fix</h1>
<p align="center">Counter-Strike 1.6 Accuracy Fix Plugin for MetaMod and ReGameDLL_CS</p>

<p align="center">
    <a href="https://github.com/SmileYzn/AccuracyFix/issues"><img alt="GitHub Issues" src="https://img.shields.io/github/issues-raw/smileyzn/AccuracyFix?style=flat-square"></a>
    <a href="https://github.com/SmileYzn/AccuracyFix/actions"><img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/SmileYzn/AccuracyFix/build.yml?branch=main&label=Build&style=flat-square"></a>
</p>

<h3>About Plugin</h3>
<p>This works with TraceLine function from Half-Life Engine, and make the default CS aim better.</p>
<p>For example, if you aim at head, that update the traceline position from attacker to head of victim player.</p>
<p>It also can control weapons recoil, but that is not the real objective of plugin!</p>

<h3>ReHLDS / ReGameDLL_CS</h3>
<p>
    This metamod plugin runs on latest action build of ReHLDS / ReGameDLL_CS versions!
    <br>
    <br>To download latest ReHLDS: <a href="https://github.com/dreamstalker/rehlds/actions?query=branch%3Amaster+is%3Asuccess+event%3Apush">Lastest Action (Master Builds) of ReHLDS here</a>
    <br>To download latest ReGameDLL_CS: <a href="https://github.com/s1lentq/ReGameDLL_CS/actions?query=is%3Asuccess+branch%3Amaster+event%3Apush">Lastest Action (Master Builds) of ReHLDS here</a>
</p>



------

<h3>Settings and variables</h3>

<details>
    <summary>Click to open</summary>
    
    // Accuracy of all weapons
    // If is set, it will replace all weapon variables
    // The default distance to fix trace line is 8192.0
    // Set to -1.0 to disable and use individual weapon values
    //
    // Default "-1.0"
    //
    af_accuracy_all     "-1.0"
    
    // Accuracy of each weapon
    // The default distance to fix trace line is 8192.0
    //
    // Default "8192.0"
    //
    af_accuracy_weapon_ak47 	"8192.0"
    af_accuracy_weapon_aug 		"8192.0"
    af_accuracy_weapon_awp 		"8192.0"
    af_accuracy_weapon_deagle 	"8192.0"
    af_accuracy_weapon_elite 	"8192.0"
    af_accuracy_weapon_famas	"8192.0"
    af_accuracy_weapon_fiveseven	"8192.0"
    af_accuracy_weapon_g3sg1 	"8192.0"
    af_accuracy_weapon_galil 	"8192.0"
    af_accuracy_weapon_glock 	"8192.0"
    af_accuracy_weapon_glock18 	"8192.0"
    af_accuracy_weapon_m249 	"8192.0"
    af_accuracy_weapon_m3 		"2020.0"
    af_accuracy_weapon_m4a1 	"8192.0"
    af_accuracy_weapon_mac10 	"8192.0"
    af_accuracy_weapon_mp5navy 	"8192.0"
    af_accuracy_weapon_p228 	"8192.0"
    af_accuracy_weapon_p90 		"8192.0"
    af_accuracy_weapon_scout 	"8192.0"
    af_accuracy_weapon_sg550 	"8192.0"
    af_accuracy_weapon_sg552 	"8192.0"
    af_accuracy_weapon_tmp 		"8192.0"
    af_accuracy_weapon_ump45 	"8192.0"
    af_accuracy_weapon_usp 		"8192.0"
    af_accuracy_weapon_xm1014 	"2020.0"
    
    // Recoil of all weapons
    // If is set, it will replace all weapon variables
    // The default recoil of an weapon is 1.0
    // Set to -1.0 to disable and use individual weapon values
    //
    // Default "-1.0"
    //
    af_recoil_all 			"-1.0"
    
    // Recoil control of each weapon
    // The default value to control recoil need to be lesss than 1.0
    // Set to -1.0 to disable and use default weapon value
    //
    // Default "1.0"
    //
    af_recoil_weapon_ak47 		"1.0"
    af_recoil_weapon_aug 		"1.0"
    af_recoil_weapon_awp 		"1.0"
    af_recoil_weapon_deagle 	"1.0"
    af_recoil_weapon_elite 		"1.0"
    af_recoil_weapon_famas		"1.0"
    af_recoil_weapon_fiveseven	"1.0"
    af_recoil_weapon_g3sg1 		"1.0"
    af_recoil_weapon_galil 		"1.0"
    af_recoil_weapon_glock 		"1.0"
    af_recoil_weapon_glock18 	"1.0"
    af_recoil_weapon_m249 		"1.0"
    af_recoil_weapon_m3 		"1.0"
    af_recoil_weapon_m4a1 		"1.0"
    af_recoil_weapon_mac10 		"1.0"
    af_recoil_weapon_mp5navy 	"1.0"
    af_recoil_weapon_p228 		"1.0"
    af_recoil_weapon_p90 		"1.0"
    af_recoil_weapon_scout 		"1.0"
    af_recoil_weapon_sg550 		"1.0"
    af_recoil_weapon_sg552 		"1.0"
    af_recoil_weapon_tmp 		"1.0"
    af_recoil_weapon_ump45 		"1.0"
    af_recoil_weapon_usp 		"1.0"
    af_recoil_weapon_xm1014 	"1.0"
    
    // Aim distance check for all weapons
    // If is set, it will replace all weapon variables
    // The default aim distance check of an weapon is 2000.0
    // Set to -1.0 to disable and use individual weapon values
    //
    // Default "-1.0"
    //
    af_distance_all 		"-1.0"
    
    // Aim distance check of each weapon
    // The default distance check aim is 8192.0
    //
    // Default "8192.0"
    //
    af_distance_weapon_ak47 	"8192.0"
    af_distance_weapon_aug 		"8192.0"
    af_distance_weapon_awp 		"8192.0"
    af_distance_weapon_deagle 	"8192.0"
    af_distance_weapon_elite 	"8192.0"
    af_distance_weapon_famas	"8192.0"
    af_distance_weapon_fiveseven	"8192.0"
    af_distance_weapon_g3sg1 	"8192.0"
    af_distance_weapon_galil 	"8192.0"
    af_distance_weapon_glock 	"8192.0"
    af_distance_weapon_glock18 	"8192.0"
    af_distance_weapon_m249 	"8192.0"
    af_distance_weapon_m3 		"8192.0"
    af_distance_weapon_m4a1 	"8192.0"
    af_distance_weapon_mac10 	"8192.0"
    af_distance_weapon_mp5navy 	"8192.0"
    af_distance_weapon_p228 	"8192.0"
    af_distance_weapon_p90 		"8192.0"
    af_distance_weapon_scout 	"8192.0"
    af_distance_weapon_sg550 	"8192.0"
    af_distance_weapon_sg552 	"8192.0"
    af_distance_weapon_tmp 		"8192.0"
    af_distance_weapon_ump45 	"8192.0"
    af_distance_weapon_usp 		"8192.0"
    af_distance_weapon_xm1014 	"8192.0"
    
</details>
