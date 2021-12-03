Creature Abilities

Ring of Fire

50 Damage every 1.4s for 7s
Animation: cast1
Start Location: Target
Radius: 4m

Water Jet

10 Damage every 0.1s for 6s
Animation: cast1
Start Location: Jaw

Breath of Fire

10 Damage every 0.1s for 6s
Animation: cast1
Start Location: Jaw

Blizzard

5 Damage every 0.1s for 14s
Animation: cast1
Start Location: Target
Radius: 5m

Lightning Discharge

25 Damage every 0.5s for 4.5s
Animation: cast1
Start Location: Target
Radius: 5m

Ice Shards

10 Damage every 0.33s for 7s
Animation: cast1
Start Location: Target
Radius: 3m

Ice Spike

20 Damage every 0.5s for 5s
Animation: cast1
Start Location: Target
Radius: 3m

Ice Tornado

10 Damage every 0.5s for 7s
Animation: cast1
Start Location: Target
Radius: 2.5

Fire Torando

10 Damage every 0.5s for 7s
Animation: cast1
Start Location: Target
Radius: 2.5

Runic Spikes

20 Damage every 0.5s for 5s
Animation: cast1
Start Location: Target
Radius: 3m

To use or customize these, you can use RRRMonsters to overide these values with the AdvancedCustomAttacks function in the JSON's it makes. Example:-

"aAdvancedCustomAttacks" : [
    {
        // Name of original Ability
        "sOriginalPrefabName" : "Spell_FireTornado_DoD",
        // Animation to use. (See RRR Doc: ConfigGuide_MonsterAnims)
        "sTargetAnim" : "cast1",
        // How often to use this ability.
        "fAIAttackInterval" : 8,
        // Prioritize the use of this ability.
        "bAIPrioritized" : true,
        // Override the base ability damage and element.
        "dtAttackDamageOverride" : {
           "fDamage":0,
           "fBlunt":0,
           "fSlash":0,
           "fPierce":0,
           "fChop":0,
           "fPickaxe":0,
           // For this example the damage is a one off impact damage.
           // The AoE that is applied is in a different script and not accessible with this JSON.
           "fFire":20,
           "fFrost":0,
           "fLightning":0,
           "fPoison":0,
           "fSpirit":0
        },
        // Override the base ability damage and keep the base element.
        "fAttackDamageTotalOverride" : null,
        // Change the projectile to use. (See RRR Doc: ConfigGuide_ProjectileNames)
        "sAttackProjectileOverride" : null,
        // Effect to use at the start of the ability, can be multiple.
        "aStartEffects" : ["SFX_Tornado_DoD", "SFX_WindblownFlame_DoD"],
        // Effect to use on hit, can be multiple.
        "aHitEffects" : ["vfx_FireballHit", "sfx_imp_fireball_explode"],
        // Effect to use on trigger, can be multiple.
        "aTriggerEffects" : ["VFX_BreathFire_DoD", "sfx_dragon_coldbreath_trailon"],
    }
]

I have left all the default values of the ability for this example.

Ability ID's

    Spell_PoisonTornado_DoD
    Spell_RingFire_DoD
    Spell_RunicSpikes_DoD
    Spell_StormBlast_DoD
    Spell_StormBolt_DoD
    Spell_StormTornado_DoD
    Spell_ArcancShot_DoD
    Spell_ArcaneBolt_DoD
    Spell_ArcaneVortex_DoD
    Spell_Blizzard_DoD
    Spell_BreathFire_Jaw_DoD
    Spell_BreathWater_Jaw_DoD
    Spell_DarkBolt_DoD
    Spell_DarkSkull_DoD
    Spell_FelVortex_DoD
    Spell_FireBolt_DoD
    Spell_FireMeteor_DoD
    Spell_FireSwirl_DoD
    Spell_FireTornado_DoD
    Spell_IceBolt_DoD
    Spell_IceShards_DoD
    Spell_IceSpike_DoD
    Spell_IceTornado_DoD
    Spell_IceTornadoAlt_DoD
    Spell_IceVortex_DoD
    Spell_LightningDischarge_DoD


Area of Effect ID's

    AoE_FireTornado_DoD
    AoE_IceShards_DoD
    AoE_IceSpike_DoD
    AoE_IceTornado_DoD
    AoE_IceTornadoAlt_DoD
    AoE_IceVortex_DoD
    AoE_LightningDischarge_DoD
    AoE_PoisonTornado_DoD
    AoE_RingFire_DoD
    AoE_RunicSpikes_DoD
    AoE_StormTornado_DoD
    AoE_ArcaneVortex_DoD
    AoE_Blizzard_DoD
    AoE_FelVortex_DoD
    AoE_FireSwirl_DoD


Projectile ID's

    Projectile_Invisible_DoD
    Projectile_Storm01_DoD
    Projectile_Storm02_DoD
    Projectile_WaterJet_DoD
    Projectile_Arcane01_DoD
    Projectile_Arcane02_DoD
    Projectile_BreathFire_DoD
    Projectile_Dark01_DoD
    Projectile_Dark02_DoD
    Projectile_Fire01_DoD
    Projectile_Fire02_DoD
    Projectile_Ice01_DoD


SFX ID's

    SFX_RoarPanther01_DoD
    SFX_RoarPanther02_DoD
    SFX_RoarQuiet01_DoD
    SFX_RoarQuiet02_DoD
    SFX_Rocks01_DoD
    SFX_RumbleDeep01_DoD
    SFX_RumbleDeep02_DoD
    SFX_RumbleDeep03_DoD
    SFX_Tornado_DoD
    SFX_WindblownFlame_DoD
    SFX_Blizzard_DoD
    SFX_Dog_DoD
    SFX_DogAttack_DoD
    SFX_DogDeath_DoD
    SFX_FrostWindBlast_DoD
    SFX_GrowlLion_DoD
    SFX_GrowlWolf_DoD
    SFX_InsectAttack01_DoD
    SFX_InsectAttack02_DoD
    SFX_InsectDeath01_DoD
    SFX_InsectDeath02_DoD
    SFX_InsectScreech01_DoD
    SFX_InsectScreech02_DoD
    SFX_LightningDischarge_DoD
    SFX_OldDog_DoD
    SFX_OldDogAttack_DoD
    SFX_OldDogDeath_DoD
    SFX_Rat_DoD
    SFX_RatAttack_DoD
    SFX_RatDeath_DoD
    SFX_RoarDeep01_DoD
    SFX_RoarDeep02_DoD
    SFX_RoarLion01_DoD
    SFX_RoarLion02_DoD
    SFX_RoarMonster01_DoD
    SFX_RoarMonster02_DoD
    SFX_RoarMonster03_DoD
    SFX_RoarMonster04_DoD
    SFX_RoarMonster05_DoD


FX Casting ID's

    FX_Casting_Fire_3_DoD
    FX_Casting_Fire_4_DoD
    FX_Casting_Fire1_DoD
    FX_Casting_Ice_2_DoD
    FX_Casting_Ice_3_DoD
    FX_Casting_Ice1_DoD
    FX_Casting_Light_2_DoD
    FX_Casting_Light1_DoD
    FX_Casting_Nature_2_DoD
    FX_Casting_Nature1_DoD
    FX_Casting_Storm_2_DoD
    FX_Casting_Storm1_DoD
    FX_Casting_Arcane_2_DoD
    FX_Casting_Arcane_3_DoD
    FX_Casting_Arcane1_DoD
    FX_Casting_Dark_2_DoD
    FX_Casting_Dark_3_DoD
    FX_Casting_Dark_4_DoD
    FX_Casting_Dark1_DoD
    FX_Casting_Fire_2_DoD


VFX Subtle ID's

    VFX_FireballShower_DoD
    VFX_FireCircle_DoD
    VFX_FireExplosion_DoD
    VFX_FireStrike_DoD
    VFX_FireSwirl_DoD
    VFX_GroundRocks_DoD
    VFX_HealingAoE_DoD
    VFX_IceBarrage_DoD
    VFX_IceGysers_DoD
    VFX_IceShardsAlt_DoD
    VFX_IceShower_DoD
    VFX_IceSpikesAlt_DoD
    VFX_IceTornado_DoD
    VFX_IceTornadoAlt_DoD
    VFX_IceVortex_DoD
    VFX_LightAura_DoD
    VFX_LightBuff_DoD
    VFX_LightHammerStrike_DoD
    VFX_LightningBlast_DoD
    VFX_LightningBoltDoD
    VFX_LightningStrike_DoD
    VFX_MushroomSpore_DoD
    VFX_PoisonStrike_DoD
    VFX_PoisonTornado_DoD
    VFX_RainOfFire_DoD
    VFX_Regeneration_DoD
    VFX_ShadowBlades_DoD
    VFX_ShadowExplosion_DoD
    VFX_Storm_DoD
    VFX_StormGround_DoD
    VFX_StormGroundPulse_DoD
    VFX_StormTornado_DoD
    VFX_Sunbeam_DoD
    VFX_ArcaneExplosion_DoD
    VFX_ArcaneStrike_DoD
    VFX_ArcaneSummon_DoD
    VFX_ArcaneVortex_DoD
    VFX_Earthquake_DoD
    VFX_EarthStrike_DoD
    VFX_FelballShower_DoD
    VFX_FelBats_DoD
    VFX_FelBreath_DoD
    VFX_FelExplosion_DoD
    VFX_FelVortex_DoD


VFX Shields ID's

    VFX_Shield_Light_DoD
    VFX_Shield_Nature_DoD
    VFX_Shield_Storm_DoD
    VFX_Shield_Arcane_DoD
    VFX_Shield_Dark_DoD
    VFX_Shield_Fire_DoD
    VFX_Shield_Ice_DoD


VFX Buffs

    VFX_Buff_Light_DoD
    VFX_Buff_Nature_DoD
    VFX_Buff_Storm_DoD
    VFX_Buff_Arcane_DoD
    VFX_Buff_Dark_DoD
    VFX_Buff_Fire_DoD
    VFX_Buff_Ice_DoD


VFX Auras

    VFX_Aura_Light_DoD
    VFX_Aura_Nature_DoD
    VFX_Aura_Storm_DoD
    VFX_Aura_Arcane_DoD
    VFX_Aura_Dark_DoD
    VFX_Aura_Fire_DoD
    VFX_Aura_Ice_DoD


VFX Explosion ID's

    VFX_Explosion_Light1_DoD
    VFX_Explosion_Light2_DoD
    VFX_Explosion_Nature1_DoD
    VFX_Explosion_Nature2_DoD
    VFX_Explosion_Storm1_DoD
    VFX_Explosion_Storm2_DoD
    VFX_Explosion_Arcane1_DoD
    VFX_Explosion_Arcane3_DoD
    VFX_Explosion_Arcane4_DoD
    VFX_Explosion_Dark1_DoD
    VFX_Explosion_Dark2_DoD
    VFX_Explosion_Dark3_DoD
    VFX_Explosion_Dark4_DoD
    VFX_Explosion_Fire1_DoD
    VFX_Explosion_Fire2_DoD
    VFX_Explosion_Fire3_DoD
    VFX_Explosion_Fire4_DoD
    VFX_Explosion_Ice1_DoD
    VFX_Explosion_Ice2_DoD
    VFX_Explosion_Ice3_DoD


VFX Stark ID's

    VFX_WaterSlash1_DoD
    VFX_WaterSlash2_DoD
    VFX_WhiffPoison_DoD
    VFX_СoldSwirl_DoD
    VFX_AbyssAOE1_DoD
    VFX_AbyssBuff_DoD
    VFX_AbyssCone_DoD
    VFX_AbyssHole_DoD
    VFX_AbyssSlash1_DoD
    VFX_AbyssSlash2_DoD
    VFX_AbyssThorns_DoD
    VFX_AbyssTornado_DoD
    VFX_AoELightning_DoD
    VFX_ArcaneRain_DoD
    VFX_BallRain_DoD
    VFX_Blizzard_DoD
    VFX_BloodExplosion_DoD
    VFX_BloodRain_DoD
    VFX_BloodSlash1_DoD
    VFX_BloodSlash2_DoD
    VFX_BloodSpikes_DoD
    VFX_BloodVortex_DoD
    VFX_BloodyPush_DoD
    VFX_BloodZone_DoD
    VFX_BreathFire_DoD
    VFX_ColdRain_DoD
    VFX_EarthSlash1_DoD
    VFX_EarthSlash2_DoD
    VFX_Fieryswirl_DoD
    VFX_Fireballs1_DoD
    VFX_Fireballs2_DoD
    VFX_FireBlast_DoD
    VFX_FireSlash1_DoD
    VFX_FireSlash2_DoD
    VFX_FireSpikes_DoD
    VFX_FireTornado_DoD
    VFX_FireWall_DoD
    VFX_FireWave_DoD
    VFX_FlyingCold_DoD
    VFX_FrostSpikes_DoD
    VFX_FrostUmbrella_DoD
    VFX_IceBlast_DoD
    VFX_IceMeteors_DoD
    VFX_IceRestoration_DoD
    VFX_IceShards_DoD
    VFX_IceSpikes_DoD
    VFX_IceStrike_DoD
    VFX_Kunai_DoD
    VFX_LightningDischarge_DoD
    VFX_MeteorRain_DoD
    VFX_NaturalSphere_DoD
    VFX_OrbAOE_DoD
    VFX_PoisonAOE_DoD
    VFX_PoisonFogDoD
    VFX_PoisonPortal_DoD
    VFX_PoisonRain_DoD
    VFX_PoisonSlash1_DoD
    VFX_PoisonSlash2_DoD
    VFX_RecoveryManna_DoD
    VFX_RingFlame_DoD
    VFX_RunicSpikes_DoD
    VFX_Shuriken_DoD
    VFX_SideSpikes_DoD
    VFX_SphereExplosion_DoD
    VFX_SphereLava_DoD
    VFX_SpikedSphere_DoD
    VFX_SplittingStones_DoD
    VFX_StoneStun_DoD
    VFX_Swamp_DoD
    VFX_WaterJet_DoD