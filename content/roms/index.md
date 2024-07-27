---
# Show the page's date?
show_date: false

# Show social sharing links?
share: false

---

# How to get started on ROMS using Poseidon
{style="text-align: left;font-size: 15pt;"}

Last updated: 2024-07-27
{style="text-align: left;font-size: 14pt;"}

## Step 1: Download the ROMS source code
{style="text-align: left;font-size: 16pt;"}

ROMS will be phasing out its subversion (SVN) repository on 2025-01-01, which is what most people up to this point have used to download and compile the ROMS source code. The source code will be made available via Git, and this is what we'll be using here.
{style="text-align: left;font-size: 14pt;"}

*All the instructions we will be following for this step are on the myroms github page: https://github.com/myroms/roms
{style="text-align: left;font-size: 14pt;"}

Prerequisites: A Poseidon account
{style="text-align: left;font-size: 14pt;"}
*You do not need to create a ROMS account to download the source code
{style="text-align: left;font-size: 14pt;"}
### 1.1. Use `git clone` to get the roms source code.
{style="text-align: left;font-size: 15pt;"}
Enter the following script, changing out `<source_dir>` for wherever you want to save the source code. If you want to save it in the directory you're currently in, don't include it.
{style="text-align: left;font-size: 14pt;"}
`git clone https://github.com/myroms/roms.git <source_dir>`
{style="text-align: left;font-size: 14pt;"}

### 1.2. Use `git clone` again to download the test cases.
{style="text-align: left;font-size: 15pt;"}
Similar to 1.1, type the following:
{style="text-align: left;font-size: 14pt;"}
`git clone https://github.com/myroms/roms_test.git <source_dir>`
{style="text-align: left;font-size: 14pt;"}

Now you should have downloaded two directories, `/roms/` and `/roms_test/`.


## Step 2: Build the executable
{style="text-align: left;font-size: 16pt;"}
In this example, we will use the <a href="https://www.myroms.org/wiki/UPWELLING_CASE">`upwelling` test case that you find on the ROMS Wiki</a>
#### 2.1. Navigate to where the upwelling test case is located
{style="text-align: left;font-size: 14pt;"}

`cd ~\roms_test\upwelling`
{style="text-align: left;font-size: 14pt;"}

#### 2.2. Edit the build script (either `build_roms.sh` or `build_roms.csh`) to point to the proper locations of your source code.
{style="text-align: left;font-size: 15pt;"}
I use `vi build_roms.sh` for this part.
{style="text-align: left;font-size: 14pt;"}

#### 2.3. Load the proper modules.
{style="text-align: left;font-size: 15pt;"}
I don't know how or why, but load ONLY these two.
{style="text-align: left;font-size: 14pt;"}

`module load stack/impi`
{style="text-align: left;font-size: 14pt;"}
`module load stack/intel`
{style="text-align: left;font-size: 14pt;"}

#### 2.4. Build the executable "romsG.exe"
{style="text-align: left;font-size: 15pt;"}
This will produce a wall of text and run for a minute or two.
`./build_roms.sh` or `./build_roms.csh`
{style="text-align: left;font-size: 14pt;"}

This will create a directory called `Build_romsG` in the `upwelling` directory, and it will contain a bunch of `.f90`, `.o`, and `.mod` files.
{style="text-align: left;font-size: 14pt;"}

