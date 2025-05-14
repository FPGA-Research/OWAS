<a href="https://www.elektronikforschung.de/projekte/di-owas"> <img src="https://github.com/user-attachments/assets/5d91b7d8-4e35-4c52-97c2-b4eb6c623895"  width=45% height=45% /> </a>
<a href="https://www.bmbf.de/DE/Home/home_node.html"> <img src="https://github.com/user-attachments/assets/8a0b7e2b-ae0e-4068-b455-600f2bafa3d0"  width=45% height=45% /> </a>


# OWAS
Entwicklung und Integration eines komplett offenen Ökosystems für den Entwurf komplexer RISC-V-basierter SoCs mit Unterstützung für eingebettete FPGAs. <br>
<a href="https://www.uni-heidelberg.de/de"> <img src="https://github.com/user-attachments/assets/098e3b87-71f7-4c5b-86d8-fb38cf753764"  width=25% height=25% /> </a>
<a href="https://www.ims.fraunhofer.de/"> <img src="https://github.com/user-attachments/assets/d43df641-3b0f-45e2-b072-5e905e6ae807"  width=32% height=32% /> </a>
<a href="https://www.ruhr-uni-bochum.de/de"> <img src="https://github.com/user-attachments/assets/6b82f4b8-4386-4f8b-a28f-0f3919ae4149"  width=27% height=27% /> </a>
<a href="https://b-horizon.com/de/"> <img src="https://github.com/user-attachments/assets/5379fb21-0eb7-4d8a-8f75-72d5d0ec8eae"  width=33% height=33% /> </a>
<a href="https://dc-vision.de/"> <img src="https://github.com/user-attachments/assets/b850bcf2-e5af-45e4-947d-9a0c5b95c388"  width=25% height=25% /> </a>
<a href="https://lubis-eda.com/"> <img src="https://github.com/user-attachments/assets/b25bff68-15a8-4fdd-9cb3-a577b920c713"  width=30% height=30% /> </a>


## Langfristiger Project-Impact
 * Offene Umgebung für adaptive RISC-V + eFPGA Systeme <br>
    (besonders robust durch Verwendung formaler Verifikationsverfahren und Post-Quantum)
 * Mehrere externe Projekte, welche DI-OWAS Tools einsetzen <br>
    FABulous wird bereits von Stanford University, Berkely, und New York University genutzt
 * FABulous als Benchmark für die Entwicklung der OpenLane Tools
 * Ausbildung von Experten (in Lehre, Summer-Schools und Tutorials)
 * Weitere Förderung für langfristige Unterstützung & Startup


## Entwurfs-Flow
<img src="https://github.com/user-attachments/assets/ee8ed425-da94-45b6-8009-d67582681cab"  width=105% height=105% /> <br>
OWAS-Container – alle notwendigen Tools in einer Box: <br>
 * Simulatoren (Verilator, Icarus Verilog, GHDL)
 * Synthese (yosys)
 * Implementierung FPGA & ASIC (nextpnr, openRoad, etc.)
 * Applikationssoftware (GCC, openOCD)
 * Zusätzliche Entwicklungstools (klayout, git, python, make, …)


## Der DI-OWAS Chip
<img src="https://github.com/user-attachments/assets/36a6c1a8-444b-4a68-b72f-47965f07ac4b"  width=100% height=100% /> <br>
 * RISC-V CPU / Prozessorsystem (basierend auf Fraunhofer IMS AIRISC-Familie)
 *   Bare-Metal-Setup oder mit eingebettetem OS (FreeRTOS / Zephyr OS)
 * Standard-Peripherie: UART, I²C, SPI, GPIO + Timer & On-Chip-Debugger
 * On-Chip RAM + Controller für externen Speicher (QSPI PSRAM / HyperRAM)
 * AXI4-basiertes Bussystem
 * FABulous eFPGA – optimierte CLBs für KI und Kryptographie
 * Dedizierte Sensorinterfaces
 * Setup für FPGA-Emulationssystem
 * Schnittstelle zu einem optionalen MPSoC-basierten Linux-Hostsystem


## Konkrete Beispielanwendungen aus dem Automotive-Bereich
 * Objekterkennung in Videostreams (Partner DC-Vision)
 * Auswertung körpernaher Sensoren (Partner B-Horizon)
 * Echtzeitfähigkeit und Sicherheit (IP Protection)


## Offene EDA-Tools und IP der Partner
 * FABulous (eFPGA Framework)
 * AIRISC (Lizenzfreier RISC-V core für FPGA und ASIC)
 * hxtorch (BrainScaleS-2 via PyTorch)


## Verwendete externe EDA-Tools und IP
 * Yosys (Logiksynthese)
 * ABC (Technology Mapping)
 * nextpnr (generisches FPGA Place&Route Tool)
 * OpenLane/OpenRoad (RTL nach GDS2 Flow)
 * PyTorch/CUDA (ML Training)
 * Ngspice (Schaltungssimulation von SPICE-Modellen)
 * RISC-V


## Kerninnovationen und Entwicklungen
 * Spezial-FPGA-Blöcke für AI und Krypto <br>
  Bislang nur einfache Arithmetik-Blöcke in FABulous<br>
  (TRL 2 &rarr; TRL 4)
 * Anwender-definierte Fabrics (Größe, Kacheln, I/O, Routing, ...) <br> 							
  Bislang nur eingeschränkte Möglichkeit für I/O und das Routing <br>
  (TRL 3 &rarr; TRL 5)
 * Automatische FPGA Werkzeuggenerierung (für die RTL-zu-Bitstream-Generierung) <br>	 	
  Bislang werden die Werkzeuge manuell an die Fabrics  angepasst <br>
  (TRL 3 &rarr; TRL 5)
 * Integrierte Werkzeuge für Optimierung und Entwurfsraumexploration <br> 			
  Bislang bedarf die Optimierung viel Expertenwissen und Eingriffe <br>
  (TRL 2 &rarr; TRL 4)
 * Integrierte Werkzeuge für Verifikation und Charakterisierung <br> 				 
  Bislang kann noch kein vollständiges Timing-Modell erzeugt werden <br>
  (TRL 3 &rarr; TRL 5)
 * System mit konfigurierbarer KI-gestützter Sensor-Fusion <br>			
  Bislang gibt es nur einfache Erkennnung ohne die geplante Unterstützung für KI und Sensor-Fusion <br>
  (TRL 2 &rarr; TRL 4)


## DI-OWAS: Projektsteckbrief
 * Projektlaufzeit:	01.05.2024 – 30.04.2027
 * Fördersumme: 	3.98M €
 * Projektansprechpartner: 
   * UH1:	<a href="https://www.ziti.uni-heidelberg.de/de/forschung/nct.html">Prof. Dirk Koch</a>; Universität Heidelberg (Koordinator) <br>
      (Im Neuenheimer Feld 386, 69120 Heidelberg)
   * UH2:	<a href="https://www.kip.uni-heidelberg.de/people/gruppe.php?action=details&num=298">PD Dr. habil. Johannes Schemmel</a>; Uni Heidelberg <br>
      (Im Neuenheimer Feld 227, 69120 Heidelberg)
   * IMS: <a href="https://www.ims.fraunhofer.de/">Stephan Nolting</a>; Fraunhofer IMS <br>
      (Finkenstraße 61, 47057 Duisburg)
   * RUB:	<a href="https://www.ruhr-uni-bochum.de/de">Prof. Tim Güneysu</a>; Ruhr-Universität Bochum <br>
      (Universitätsstr. 150, 44801 Bochum)
   * BH:	<a href="https://b-horizon.com/de/">Mohammad Kabany</a>; B-Horizon GmbH <br>
      (Bruckdorfer Str. 34, 93161 Sinzing)
   * LU:	<a href="https://lubis-eda.com/about-us/">Dr. Max Birtel</a> ; LUBIS EDA GmbH <br>
      (Trippstadter Straße 110, 67663 Kaiserslautern)
   * DCV:	<a href="https://dc-vision.de/">Frederik Lange</a>; DC Vision Systems GmbH <br>
      (Rollnerstraße 59, 90408 Nürnberg)
 * Kontakt:    dirk.koch@uni-heidelberg.de



