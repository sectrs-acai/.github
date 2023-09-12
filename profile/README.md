# Protecting Accelerator Execution with Arm Confidential Computing Architecture

## Abstract 
Trusted execution environments in several existing and upcoming CPUs demonstrate
the success of confidential computing, with the caveat that tenants cannot use
accelerators such as GPUs and FPGAs. Even after hardware changes to enable TEEs
on both sides and software changes to adopt existing code to leverage these
features, it results in redundant data copies and hardware encryption at the
bus-level and on the accelerator thus degrading the performance and defeating
the purpose of using accelerators. In this paper, we reconsider the Arm
Confidential Computing Architecture (CCA) design — an upcoming TEE feature in
Arm v9 — to address this gap. We observe that CCA offers the right abstraction
and mechanisms to allow confidential VMs to use accelerators as a first class
abstraction, while relying on the hardware-based memory protection to preserve
security. We build ACAI, a CCA-based solution, to demonstrate the feasibility of
our approach while addressing several critical security gaps. Our experimental
results on GPU and FPGA show that ACAI can achieve strong security guarantees
while maintaining performance and compatibility.


```
@misc{sridhara2023acai,
      title={ACAI: Extending Arm Confidential Computing Architecture Protection from CPUs to Accelerators}, 
      author={Supraja Sridhara and Andrin Bertschi and Benedict Schlüter and Mark Kuhne and Fabio Aliberti and Shweta Shinde},
      year={2023},
      eprint={2305.15986},
      archivePrefix={arXiv},
      primaryClass={cs.CR}
}
```

https://github.com/sectrs-acai/acai/
https://sectrs.ethz.ch/
