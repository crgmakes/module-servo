# Servo Module

All the source files for the servo module hardware.

# Software 

You will need [KiCad](https://kicad.org) to view and edit this design. Click [here](https://www.kicad.org/download/) to download.

You will also need all the associated libraries and models to drive the design if you want to make changes or view the 3D rendering:

https://github.com/crgmakes/kicad-library.git

Kicad MUST be configured properly to use all the files in this repo. Once you have Kicad installed, under Preferences->Configure Paths..., make the following entries:

1. KICAD_USER_DIR -> set to the root location of where you placed the above repository.
2. KICAD_USER_LIBRARY = ${KICAD_USER_DIR}/Library
3. KICAD_USER_MODEL_DIR = ${KICAD_USER_LIBRARY}/models
4. KICAD_USER_TEMPLATE_DIR = ${KICAD_USER_LIBRARY}/templates	

Kicad will operate mostly normally if these are not set properly. You will notice an issue when you view the PCB in 3D mode.

***NOTE***: after makeing a release build in git, if your rendered 3D images are missing components, ensure the path to EVERY component model is set to ${KICAD_USER_MODEL_DIR}/<model name>.

Kicad sometimes replaces the variable with an expansion and that FAILS during the build process because the expanded variable is local and does not match the build environment.

---

THE DESIGN IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS DESIGN INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS DESIGN.