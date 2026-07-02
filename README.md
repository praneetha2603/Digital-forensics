# 🔍 Blackwood Ripper: Digital Forensics Investigation

## 📖 Overview

The Blackwood Ripper investigation is a fictional end-to-end digital forensics case study designed to simulate a real-world cybercrime investigation involving malware-enabled surveillance, command-and-control infrastructure, digital stalking, and forensic evidence recovery.

The objective of this project was to reconstruct attacker activity and establish attribution by correlating evidence obtained from memory forensics, disk forensics, malware analysis, browser artifacts, and removable media analysis.

---

## 🛠 Tools Used

- Volatility 3
- Magnet AXIOM
- Autopsy
- FTK Imager

---

## 🎯 Investigation Workflow

### Phase 1: Victim System Analysis

The investigation began with the discovery of **Sarah K., a forest ranger**, who was found dead under suspicious circumstances. Her laptop was seized and subjected to forensic examination.

Memory analysis using Volatility revealed multiple instances of:

```text
wscript.exe
```

executing a malicious VBScript file:

```text
SystemMonitor.vbs
```

indicating active script-based malware operating on the victim machine.

---

### Phase 2: Malware Persistence and Surveillance

Disk analysis using Magnet AXIOM confirmed the existence of the malware in multiple locations, including temporary directories and Windows startup locations.

Recovered artifacts demonstrated persistence mechanisms designed to survive reboots and maintain continuous execution.

The malware was found capturing screenshots and storing them under locations such as:

```text
ProgramData\SystemMonitor\screenshots
```

Additional logs including:

```text
monitor_log.txt
```

confirmed continuous monitoring and collection of victim activity.

These findings established that Sarah's system was under active surveillance without her knowledge.

---

### Phase 3: Command and Control Attribution

Network artifacts recovered from the victim machine revealed communication with an external command-and-control endpoint.

Further investigation linked the infrastructure to the primary suspect:

## Marcus Blackwood

This marked the transition from victim analysis to suspect attribution.

---

### Phase 4: Suspect Laptop Analysis

Forensic examination of Marcus Blackwood's laptop uncovered a dedicated command-and-control environment located at:

```text
C:\forensics\C_2_Server\
```

The following artifacts were recovered:

- `beacons.txt`
- `heartbeats.txt`
- `data.txt`

These files indicated active communication and telemetry collection from infected systems.

Investigators additionally recovered:

```text
c2_server.py
```

which confirmed the operation of a custom Python-based C2 server used to control malware deployments and receive exfiltrated data.

Screenshot archives recovered from the suspect machine contained images captured directly from victim systems, proving successful surveillance and data theft.

---

### Phase 5: Behavioral and Browser Artifact Analysis

Browser history analysis revealed searches relating to:

- methods of committing murder
- removing blood traces and footprints
- changing location data
- serial killer behavioral patterns
- police investigation techniques

Investigators also discovered repeated visits to social media profiles belonging to multiple victims, indicating stalking activity prior to the crimes.

Additional evidence showed searches and purchases related to gloves and other materials intended to reduce forensic trace evidence.

Several of these artifacts were recovered from deleted browser records, suggesting deliberate attempts to conceal evidence.

---

### Phase 6: USB Forensic Analysis

Analysis of Marcus Blackwood's USB drive using Autopsy revealed several critical findings:

- keyword hits containing **"blackwood ripper"**
- images of jewelry believed to be trophies collected from victims
- encrypted files intended to conceal evidence
- a deleted manuscript describing the murders

These artifacts provided direct evidence of planning, execution, and documentation of criminal activity.

---

## 📌 Final Conclusion

The investigation established that Marcus Blackwood orchestrated a sophisticated surveillance campaign by deploying malware to victim systems.

The malware enabled remote monitoring through screenshot capture, activity logging, and data exfiltration to a custom command-and-control server operated by the suspect.

Evidence recovered from memory analysis, disk artifacts, browser history, and removable media demonstrated stalking behavior, operational planning, forensic evasion attempts, and post-compromise data collection.

The combined findings from Volatility, Magnet AXIOM, and Autopsy provided a complete evidentiary chain linking Marcus Blackwood to the crimes associated with the Blackwood Ripper case.

---

## 📂 Repository Contents

```text
Digital-forensics/
│
├── evidence/
│   └── README.md              # Evidence download instructions
│
├── final digital forensics report.pdf
│
└── README.md
```

---

## 📦 Evidence Files

Due to GitHub file size limitations, forensic artifacts are hosted externally.

The evidence package contains:

- `saras.raw`
- `marcus.raw`
- `SARAS-20260405-211956.dmp`
- `USB CONTENT`
- `investigation.html`

See:

```text
evidence/README.md
```

for download instructions.

---

## ⚠ Disclaimer

This project is entirely fictional and was created for educational, research, and portfolio purposes only.

The evidence package may contain malware samples and malicious artifacts intended solely for forensic analysis in controlled environments.

No real individuals, organizations, or criminal events are represented.
