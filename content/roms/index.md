---
# Show the page's date?
show_date: false

# Show social sharing links?
share: false

---

# How to get started on ROMS using Poseidon

Last updated: 2024-07-27

## Step 1: Download the ROMS source code

ROMS will be phasing out its subversion (SVN) repository on 2025-01-01, which is what most people up to this point have used to download and compile the ROMS source code. The source code will be made available via Git, and this is what we'll be using here.
{style="text-align: left;font-size: 14pt;"}

*All the instructions we will be following for this step are on the myroms github page: https://github.com/myroms/roms
{style="text-align: left;font-size: 14pt;"}

Prerequisites:
* A Poseidon account
{style="text-align: left;font-size: 14pt;"}

*You do not need to create a ROMS account to download the source code
{style="text-align: left;font-size: 14pt;"}

## Step 2: Building the upwelling test case
#### 1. Navigate to where the upwelling test case is located
{style="text-align: left;font-size: 14pt;"}

`cd ~\roms_test\upwelling`
{style="text-align: left;font-size: 14pt;"}

#### 2. Edit the build script (either `build_roms.sh` or `build_roms.csh`) to point to the proper locations of your source code.
{style="text-align: left;font-size: 14pt;"}
I use `vi build_roms.sh` for this part.
{style="text-align: left;font-size: 14pt;"}

#### 3. Load the proper modules.
{style="text-align: left;font-size: 14pt;"}
I don't know how or why, but load ONLY these two.
{style="text-align: left;font-size: 14pt;"}

`module load stack/impi`
{style="text-align: left;font-size: 14pt;"}

`module load stack/intel`
{style="text-align: left;font-size: 14pt;"}

#### 4. Build the executable "romsG.exe"
{style="text-align: left;font-size: 14pt;"}
`./build_roms.sh` or `\build_roms.csh`
{style="text-align: left;font-size: 14pt;"}

