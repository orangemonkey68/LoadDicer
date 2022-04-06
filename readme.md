# LoadDicer
Nobody likes waiting for their games to load!

## Q/A:

### Q: What is it?
**A**: LoadDicer aims to parallelize `Registry` in an effort to drastically reduce load times in large modpacks.

### Q: Can I use this in a small / vanilla-like pack?
**A**: Yes.  
**Long answer**: Yes, but it'll have very little performance impact. The way that LoadDicer generates threads is **per-mod**, 
yielding little impact in a small pack.

### Q: Can you port this to Forge?
**A**: No. Not because I despise Forge, I just know very little about it. If you are a developer and know a good 
amount about Forge developing, reach out to me on Discord `@s0vi_#1312`

## Roadmap
- [ ] Alpha
    - [ ] CI / CD
    - [ ] Fully understand `Registry`, and it's subclasses
    - [ ] Implement an `AsyncRegistry`, verify complete compatibility in vanilla
    - [ ] Implement a `RegistryController`, implement per-mod threading
- [ ] Beta
    - [ ] Write CI / CD to auto-test top 100 mods on commit
    - [ ] Test top 100 (co-compatible) mods, detail which cause errors
    - [ ] Fix compatibility errors, to whatever degree possible
    - [ ] Investigate supporting custom registries (looking at you, TechReborn)
- [ ] Release
    - [ ] Fix bugs 
    - [ ] Investigate using other methods to assign work to each thread (besides per-mod)
    - [ ] Only the future knows :-)
    


