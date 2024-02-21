# requirements
- bash and a unix based system(wsl works too.)
- shnsplit
- ffmpeg
- cuetag
- ## the correct structure:
    - must have split raw music files(eg. multiple flac/ape/m4a files) or a simple raw album file(.ape or .flac) and an accompanying .cue file(must exist) in the same directory like the below:
    ```
    1999 - Nattestid Ser Porten Vid
    ├── Folder.auCDtect.txt
    ├── front.jpg
    ├── Scans
    │   ├── Taake___Nattestid___Back.jpg
    │   ├── Taake___Nattestid___CD.jpg
    │   ├── Taake___Nattestid___Front.jpg
    │   ├── Taake___Nattestid___Inside01.jpg
    │   ├── Taake___Nattestid___Inside02.jpg
    │   └── Taake___Nattestid___Inside03.jpg
    ├── Taake - Nattestid Ser Porten Vid.ape
    ├── Taake - Nattestid Ser Porten Vid.cue
    └── Taake - Nattestid Ser Porten Vid.log
    ```
    of course, this structure works as well:
    ```
    2019 - METAL GALAXY [JP]
    ├── 1-01. FUTURE METAL.flac
    ├── 1-02. DA DA DANCE (feat. Tak Matsumoto).flac
    ├── 1-03. Elevator Girl.flac
    ├── 1-04. Shanti Shanti Shanti.flac
    ├── 1-05. Oh! MAJINAI (feat. Joakim Brodén).flac
    ├── 1-06. Brand New Day (feat. Tim Henson and Scott LePage).flac
    ├── 1-07. ↑↓←→BBAB.flac
    ├── 1-08. Night Night Burn!.flac
    ├── 2-01. IN THE NAME OF.flac
    ├── 2-02. Distortion (feat. Alissa White-Gluz).flac
    ├── 2-03. PA PA YA!! (feat. F.HERO).flac
    ├── 2-04. BxMxC.flac
    ├── 2-05. Kagerou.flac
    ├── 2-06. Starlight.flac
    ├── 2-07. Shine.flac
    ├── 2-08. Arkadia.flac
    └── cover.jpg
    ```
# how to use it:
Simply run the script with the album's relative or absolute path being provided as a parameter:
```
cdsplit.py "~/Music/Lustre/2020 - The Ashes Of Light"
```
the script also has some additional flags which can be used to change the format and bitrate among other things, simply use the -h flag to see them.
