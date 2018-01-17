# PILOT-TRENTO
Repository representing the customizations, specific extensions, and features of Trento SIMPATICO Pilot

## Pilot Deployment
### Components
The following components are engaged
- AAC (aac)
- LOG (logs)
- Citizenpedia
- TAE (simpatico-adaptation-engines)
- WAE (simpatico-adaptation-engines)
- CPD 
- CDV
- IFE
- Dashboard

### Physical deployment
- Main linux server ``simpatico.smartcommunitylab.it`` hosting most of the components (LOG, Citizenpedia, TAE, WAE, CPD, Dashboard). Access to the components id managed by ``Apache Web server``.
- CDV is deployed on Trento municipality premises.
- For complex text processing experiments the FBK server is engaged.

## Pilot-specific Customizations
### AAC
- For the user authentication purposes specific identity providers are involved: CPS (Trento province level) and SPID (Italian national identity system). Both providers may give access to specific information: age, place of birth, residence. The providers are used also by the portal where e-services are involved and SSO implemented.
- Google is used as alternative.

### IFE
Customizations refer to
- SIMPATICO Toolbar (layout and styling)
- Components engaged (WAE, TAE as popup tool, Citizenpedia, CPD, CDV)
- Introductory tutorial

### TAE
- Only Italian language is currently used for the pages
- TAE is invoked as a popup tool (selecting a word or a phrase to explain)

## Logged Events

- For session
  - sessionstart
  - formstart
  - sessionend
  - generic (ife, duration, session)
  - formend
  - generic (ife, duration, form)
  
- For WAE 
  - wae
  - generic (wae, simplification_start)
  - generic (wae, block_start)
  - generic (wae, duration, block)
  - generic (wae, block_end)
  - generic (wae, duration, simplification)
  - generic (wae, simplification_end)

- For TAE
  - generic (tae, simplification_start)
  - tae/freetext
  - tae/word
  - generic (tae, viewsimp)
  - generic (tae, dosimp)
  - generic (tae, viewdef)
  - generic (tae, dodef)
  - generic (tae, viewwiki)
  - generic (tae, dowiki)
  - generic (tae, duration, simplification)
  - generic (tae, simplification_end)
  
- For CTZ
  - generic (ctz, simplification_start)
  - ctzp/contentrequest
  - ctzp/questionrequest
  - ctzp/newquestion
  - generic (ctz, duration, simplification)
  - generic (ctz, simplification_end)
  
- For CPD
  - generic (cpd, process_start)
  
- For CDV
  - generic (cdv, usedata)
  - generic (cdv, savedata)
  



