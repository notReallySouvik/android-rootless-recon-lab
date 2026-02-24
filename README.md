# Android Rootless Recon Lab

A structured, modular penetration testing laboratory built on a rootless Debian environment running on Android.  
This project provides an academic and practical framework for setting up, organizing, automating, and documenting security tools within a controlled lab environment.

---

## 1. Overview

The Android Rootless Recon Lab is designed to:

- Deploy a Debian-based Linux userland on Android without root privileges
- Organize penetration testing tools into structured categories
- Provide documented installation and usage guides for each tool
- Automate tool deployment using a centralized control script
- Maintain academic documentation of design, architecture, and constraints

This repository is intended for **educational and research purposes only**.

---

## 2. Objectives

The primary goals of this project are:

1. To demonstrate how a portable penetration testing lab can be deployed on Android.
2. To categorize tools in a structured and maintainable format.
3. To automate installation using a master control script.
4. To document architectural decisions and system limitations academically.
5. To provide a scalable framework for future expansion.

---

## 3. Repository Structure

android-rootless-recon-lab/
│
├── README.md
├── LICENSE
├── setup/
├── tools/
├── core/
├── docs/
└── screenshots/


### 3.1 `setup/`
Contains step-by-step environment setup documentation:

- Base environment preparation
- Debian (proot) configuration
- GUI configuration (optional)
- Custom launcher aliases
- Storage mounting
- Troubleshooting notes

### 3.2 `tools/`
Category-wise structured documentation of tools.

Each tool is organized into its own directory:

tools/
└── Category_Name/
└── tool_name/
├── README.md
├── installation.md
└── usage.md


Tool documentation includes:
- Purpose and functionality
- Installation steps
- Basic usage examples
- Notes and limitations

### 3.3 `core/`
Contains automation and orchestration scripts.

Includes:
- `master_lab.sh` – central control script
- `modules/` – installation engine and helper scripts
- `tool_registry/` – category-wise tool lists

This component enables automated tool installation and structured expansion.

### 3.4 `docs/`
Academic documentation of the project:

- Background
- Problem statement
- Architecture
- Constraints
- Design decisions
- Implementation
- Limitations
- Future work
- Threat model
- Data flow diagram

This section supports formal submission or technical review.

### 3.5 `screenshots/`
Visual references of:
- Environment setup
- Tool execution
- GUI configuration (if applicable)

---

## 4. System Architecture (High-Level)

The lab operates in the following layers:

1. Android Host System  
2. Rootless Linux Userland (Debian via proot)  
3. Categorized Tool Environment  
4. Automation Layer (Master Control Script)  
5. Documentation and Reporting Layer  

The architecture prioritizes:
- Portability
- Modularity
- Scalability
- Maintainability

---

## 5. Tool Categorization

Tools are grouped into structured categories including:

- Information Gathering  
- Vulnerability Analysis  
- Web Application Analysis  
- Database Assessment  
- Password Attacks  
- Wireless Attacks  
- Reverse Engineering  
- Exploitation Tools  
- Sniffing and Spoofing  
- Post Exploitation  
- Forensics  
- Reporting Tools  
- Social Engineering  

Each category is modular and extendable.

---

## 6. Installation Workflow

High-level process:

1. Configure Android environment  
2. Install Debian userland  
3. Configure storage and networking  
4. Run master control script  
5. Select desired tool categories  
6. Automated installation and setup  

Detailed instructions are available in the `setup/` directory.

---

## 7. Constraints

- No root access required
- Limited by Android kernel capabilities
- Hardware-dependent performance
- GUI optional and resource-intensive
- Some tools may require architecture-specific adjustments

Refer to `docs/04_constraints.md` for detailed analysis.

---

## 8. Ethical Use Notice

This repository is intended strictly for:

- Academic research
- Cybersecurity education
- Authorized penetration testing
- Controlled lab experimentation

Unauthorized use of the tools documented here against systems without explicit permission is illegal and unethical.

The authors assume no liability for misuse.

---

## 9. License

This project is distributed under the MIT License.  
See the `LICENSE` file for details.

---

## 10. Future Work

Planned improvements include:

- Enhanced automation logic
- Architecture-aware installer refinement
- Scenario-based lab exercises
- Containerization experiments
- Performance optimization studies

---

## 11. Contribution Guidelines

Contributions should:

- Follow existing directory structure
- Maintain academic writing tone
- Avoid duplication of tools
- Include installation and usage documentation
- Respect licensing constraints of third-party tools

---

## 12. Disclaimer

Some referenced tools may be:
- Commercial
- Restricted-license
- Platform-specific

This repository does not redistribute proprietary software.  
It documents installation and usage procedures only.

---

## Author

Souvik Das  
Independent Academic Project
Android Rootless Recon Lab  
Year: 2026