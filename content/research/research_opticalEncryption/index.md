---
date: "2013-06-01T00:00:00Z"
# external_link: "https://ysabelwang.github.io/project/gom_sst/"
# image:
#  caption: Data obtained from [GHRSST OSTIA L4 SST Analysis](doi.org/10.5067/GHOST-4FK01)
#  focal_point: Smart
#links:
# - icon: twitter
#   icon_pack: fab
#   name: Follow
#   url: https://twitter.com/georgecushen
# slides: example
#summary: 

tags:
#- SST
#- NetCDF
#- MATLAB
#- Gulf of Mexico
title: Optical Encryption
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""


# Show the page's date?
show_date: false

# Show social sharing links?
share: false
---
For my undergraduate thesis, I developed a numerical optical encryption method that combined phase retrieval and chaos theory to secure digital images. In this method, the plaintext (the image to be encrypted) is propagated  via Rayleigh-Sommerfled diffraction a set distance, after which it is modulated with a phase mask generated using a chaos equation. This is repeated for another distance and another chaos-generated phase mask. Using a simulated diffuser with its own chaos-generated phase distributions, the intensity of the encrypted plaintext is captured, resulting in a ciphertext (the fully encrypted image) with no phase information.
{style="text-align: left;font-size: 14pt;"}

To decrypt the ciphertext, all encryption keys (ie., parameters used during encryption) and their order of execution must be known, including the constants used to generate the chaos phase masks. Minimal changes to any of the keys resulted in decryption failure, proving the system's sensitivity and robustness.
{style="text-align: left;font-size: 14pt;"}

