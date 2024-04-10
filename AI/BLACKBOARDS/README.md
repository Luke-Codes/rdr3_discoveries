## Some Blackboard Values

Visible changes can only be seen with few "script" blackboards. It seems Rockstars use blackboards as decorators to check some actions status.

## Example

```lua
	-- SET_PED_BLACKBOARD_FLOAT (visible changes only for "script" blackboards)
	-- to cancel blackboard float use value 0.0
	-- last parameter is duration (in frames, -1 = forever)
	Citizen.InvokeNative(0x437C08DB4FEBE2BD, PlayerPedId(), "MetalDetectorDetectionValue", 1.0, -1)   -- the higher the value, the more metal detector vibrates

	-- SET_PED_BLACKBOARD_BOOL (visible changes only for "script" blackboards)
	-- last parameter is duration (in frames, -1 = forever)
	Citizen.InvokeNative(0xCB9401F918CB0F75, PlayerPedId(), "NarrowLedge", true, 1000)  -- apply "narrow" walkstyle for 1000 frames (~10 seconds)

	-- SET_PED_BLACKBOARD_STRING (visible changes only for "script" blackboards)
	-- last parameter is duration (in frames, -1 = forever)
	Citizen.InvokeNative(0xA762C9D6CF165E0D, PlayerPedId(), "BodyPartChained", "Legs", 5000)  -- apply "legschained" walkstyle for 5000 frames (~50 seconds)

	-- SET_PED_BLACKBOARD_INT
	-- last parameter is duration (in frames, -1 = forever)
	-- in this example the native N_0x2e036f0480b8bf02() returns the amount of time elapsed since joining game
	Citizen.InvokeNative(0x5F53010C4C3F6BAF, PlayerPedId(), "prsn_ilo_time", N_0x2e036f0480b8bf02(), -1)  --

```

<h2>Some known Blackboard Values.</h2>

-Blackboard type | Blackboard section | Blackboard name | Blackboard range (or variants)
----------- | -------------------------- |---------- | -------
float | script | Cautious | from 0.1 till 1.0
float | script | Stealth | from 0.1 till 1.0
float | script | Bewildered | from 0.1 till 1.0
float | script | MetalDetectorDetectionValue | from 0.1 till 1.0
float | script | Sick | from 0.7 till 1.0
float | script | Stealth | from 0.1 till 1.0
bool | script | Bewildered |
bool | script | blockHeadTailAdditives |
bool | script | CarryBagAndersLeft |
bool | script | CarryBagAndersRight |
bool | script | CarryFishingpole |
bool | script | CarryManure |
bool | script | Cold_Empty_Stamina |
bool | script | Cold_Low_Stamina |
bool | script | Cold_Stamina |
bool | script | Crafting_SatchelUpgrade |
bool | script | DoHerdSmack |
bool | script | DoHerdWhip |
bool | script | DrunkStumbleActive |
bool | script | FishingRodInLeftHand |
bool | script | FishingRodInRightHand |
bool | script | ForceHandsOnBelt |
bool | script | FreeRoamSpawn |
bool | script | GRAYOUT_ITEM_DROP |
bool | script | GRAYOUT_ITEM_USE |
bool | script | HandsOnBelt |
bool | script | Handsup |
bool | script | in_a_dress |
bool | script | inInspectionMode |
bool | script | IsCold |
bool | script | IsColdFast |
bool | script | isInspectingGround |
bool | script | isLowDeadEyeCoreActive |
bool | script | isLowHealthCoreActive |
bool | script | isLowStaminaCoreActive |
bool | script | IsSearching |
bool | script | IsSeductive |
bool | script | IsWithinHornetsVolume |
bool | script | LanternHeldHigh |
bool | script | MP_Style_Casual |
bool | script | MP_Style_Crazy |
bool | script | mp_style_drunk |
bool | script | MP_Style_EasyRider |
bool | script | MP_Style_Flamboyant |
bool | script | MP_Style_Greenhorn |
bool | script | MP_Style_Gunslinger |
bool | script | mp_style_inquisitive |
bool | script | MP_Style_Refined |
bool | script | MP_Style_SilentType |
bool | script | MP_Style_Veteran |
bool | script | NarrowLedge |
bool | script | odr3_basement |
bool | script | odr3_outside |
bool | script | OnFootIntimidateForced |
bool | script | PickUpManure |
bool | script | PlayEquipGlovesFidget |
bool | script | PlayEquipHatFidget |
bool | script | PlayLeadin |
bool | script | PlayUnequipGlovesFidget |
bool | script | PlayUnequipHatFidget |
bool | script | PutDownManure |
bool | script | SadPassenger |
bool | script | SpawnMissionIntro |
bool | script | Urgent_Look_Back |
bool | script | Urgent_Look_Left |
bool | script | UrgentGlances |
string | script | BodyPartChained | Legs
bool |  | BlockInjuredLoco |
bool |  | DoAFidget |
bool |  | DoBulletFlinch |
bool |  | DoLowStarts |
bool |  | EagleEye |
bool |  | FoliageActive |
bool |  | frontpassenger |
bool |  | HandsOnBelt |
bool |  | Handsup |
bool |  | HorseLeadingActive |
bool |  | InCombat |
bool |  | IsAiming |
bool |  | IsAimingMounted |
bool |  | IsClimbExit |
bool |  | IsDoingItemInteraction |
bool |  | IsDrunk |
bool |  | IsEnteringCover |
bool |  | IsFocusTarget |
bool |  | IsInInterior |
bool |  | isInspecting |
bool |  | IsLanding |
bool |  | isLowStaminaCoreActive |
bool |  | IsOnFire |
bool |  | IsPlayer |
bool |  | OnFootIntimidate |
bool |  | onStairs |
bool |  | passenger |
bool |  | PedIsWearingHat |
bool |  | Rider |
bool |  | RiderAiming |
bool |  | RiderBlockIdleVariations |
bool |  | RiderDoWhip |
bool |  | RiderIntensityHigh |
bool |  | RideSideSaddled |
bool |  | Spooked |
bool |  | Tracking |
float |  | SurfaceIncline | from -3.2 till 3.14
float |  | Agitation | from 0.1 till 1.0
float |  | BulletFlinchDirection | from -3.2 till 3.14
float |  | cautious | from 0.1 till 1.0
float |  | ClimbHeight | from 0.75 till 3.5
float |  | Drunkness | from 0.1 till 1.0
float |  | Fatigue | from 0.1 till 1.0
float |  | Fear | from 0.1 till 1.0
float |  | FireDistance | from 0.1 till 4.5
float |  | FoliageHeight | from 0.3 till 10.0
float |  | Injury | from 0.001 till 1.0
float |  | ShuntAngle | from -3.1425 till 3.1425
float |  | ShuntForce | from 0.05 till 1.0
float |  | Soak | from 0.1 till 1.0
float |  | Strain | from 0.1 till 1.0
float |  | Temperature | from -50.0 till 1000.0
float |  | Unruliness | from 0.1 till 1.01
float |  | WaterDepth | from 0.1 till 2.0
float |  | WindSpeed | from 1.0 till 100.0
float |  | StaminaCoreValue | from 0.0 till 40.0
float |  | HealthCoreValue | from 0.0 till 40.0
float |  | rain | from 0.1 till 1.0
bool |  | BLOCK_CAMERA_DRUNK_SLUMP_BEHAVIOUR |
bool |  | BLOCK_COFFEE_DISCARD_PROMPT |
bool |  | BLOCK_COFFEE_DRINK_PROMPT |
bool |  | BLOCK_STEW_DROP_PROMPT |
bool |  | BLOCK_STEW_EAT_PROMPT |
bool |  | BOOK_BLOCK_PAGE_NEXT |
bool |  | BOOK_BLOCK_PAGE_PREV |
bool |  | DoAFidget |
bool |  | DoLowStarts |
bool |  | FreeRoamSpawn |
bool |  | GENERIC_ALCOHOL_ALLOW_CHUG_B |
bool |  | GENERIC_ALCOHOL_ALLOW_CHUG_C |
bool |  | GENERIC_ALCOHOL_BLOCK_AWAY_PROMPT |
bool |  | GENERIC_ALCOHOL_BLOCK_CHEERS_HI_DISCARD |
bool |  | GENERIC_ALCOHOL_BLOCK_CHEERS_HI_PUTAWAY |
bool |  | GENERIC_ALCOHOL_BLOCK_CHEERS_LO |
bool |  | GENERIC_ALCOHOL_BLOCK_CHUG_A |
bool |  | GENERIC_ALCOHOL_BLOCK_CHUG_DISCARD |
bool |  | GENERIC_ALCOHOL_BLOCK_CHUG_PUT_AWAY |
bool |  | GENERIC_ALCOHOL_BLOCK_DISCARD_PROMPT |
bool |  | GENERIC_ALCOHOL_BLOCK_PUTAWAY_PROMPT |
bool |  | GENERIC_BOOK_READ_AVAILABLE |
bool |  | GENERIC_BOOK_RETURN_AVAILABLE |
bool |  | GENERIC_BOOK_TAKE_AVAILABLE |
bool |  | GENERIC_DOCUMENT_FLIP_AVAILABLE |
bool |  | GENERIC_WEAPON_CLEAN_PROMPT_AVAILABLE |
bool |  | HIDE_STEW_DROP_PROMPT |
bool |  | HIDE_STEW_EAT_PROMPT |
bool |  | InCombatCharging |
bool |  | inInspectionMode |
bool |  | isInspectingGround |
bool |  | isLowDeadEyeCoreActive |
bool |  | isLowHealthCoreActive |
bool |  | isLowStaminaCoreActive |
bool |  | JOURNAL_BLOCK_CHAPTER_NEXT |
bool |  | JOURNAL_BLOCK_CHAPTER_PREV |
bool |  | JOURNAL_BLOCK_PAGE_NEXT |
bool |  | JOURNAL_BLOCK_PAGE_PREV |
bool |  | Loco::UseActionMode |
bool |  | MP_CATALOGUE_BLOCK_PAGE_NEXT |
bool |  | MP_CATALOGUE_BLOCK_PAGE_PREV |
bool |  | PlayEquipGlovesFidget |
bool |  | PlayEquipHatFidget |
bool |  | PlayUnequipGlovesFidget |
bool |  | PlayUnequipHatFidget |
bool |  | POILookAround |
bool |  | POILookDown |
bool |  | POILookInto |
bool |  | RequestKneeCrouch |
bool |  | SHOW_COFFEE_KNEEL_DISCARD_PROMPT |
bool |  | SideSaddleRider |
bool |  | SpawnMissionIntro |
bool |  | UseFacing |
float |  | MetalDetectorDistanceToDigSite |
string |  | DecelerationCause | stopping
string |  | EmotionalState | CombatMediumIntensity<br>CombatHighIntensity<br>cautious<br>HighIntensitySearch<br>cower<br>panic<br>angry<br>LowIntensitySearch<br>scared<br>IntimidatedOnFeet<br>Curious<br>Nervous<br>itchy<br>sad<br>shocked<br>brave<br>happy
string |  | IsAboutToRansackIdleType | ReachInPickup<br>ReachOverPickup
string |  | Stance | normal<br>action
string |  | StrafeType | Aiming<br>Fishing<br>melee<br>OffsetAiming
string |  | typeOfGetUp | front<br>rear
string |  | WeatherType | blizzard<br>drizzle<br>groundblizzard<br>highpressure<br>hurricane<br>rain<br>sandstorm<br>shower<br>sleet<br>snow<br>snowlight<br>sunny<br>thunderstorm<br>whiteout
string |  | MoodName | MoodAction<br>MoodAgitated<br>MoodAgitatedLow<br>MoodAngry<br>MoodBlizzard<br>MoodBrave<br>MoodCalmHorse<br>MoodCarryLarge<br>MoodCautious<br>MoodCold<br>MoodCombatMedium<br>MoodCombatMild<br>MoodConfused<br>MoodCower<br>MoodCurious<br>MoodDisgust<br>MoodDrunkExtreme<br>MoodDrunkMedium<br>MoodDrunkMild<br>MoodExertionextreme<br>MoodExertionmedium<br>MoodExertionmild<br>MoodExhausted<br>MoodFoliage<br>MoodHappy<br>MoodInjuredExtreme<br>MoodInjuredMedium<br>MoodInjuredmild<br>MoodIntimidated<br>MoodInvestigate<br>MoodLowDeadeye<br>MoodLowHealth<br>MoodLowStamina<br>MoodNervous<br>MoodNormal<br>MoodNormalCanter<br>MoodNormalSick<br>MoodNormalTrot<br>MoodOnFire<br>MoodPanic<br>MoodRiding<br>MoodRidingRelaxed<br>MoodRun<br>MoodSad<br>MoodScared<br>MoodSearchHigh<br>MoodSearchLow<br>MoodSeductive<br>MoodShocked<br>MoodSlide<br>MoodSmug<br>MoodSwamp<br>MoodTired<br>MoodUnderfireHeavy<br>MoodUnderfireMild<br>MoodWater<br>MoodWindExtreme<br>MoodWindMedium<br>MoodWindMild
int |  | prsn_ilo_time |