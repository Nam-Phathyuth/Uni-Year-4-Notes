# 2.1 Layered Technology
## a.  process, methods, and tools
![[Drawing 2023-10-09 22.04.32.excalidraw.png]]
- the foundation for SE is the *process layer*. **SE** process is the glue that hold the technology layer together and enable rational and timely develop of computer software
- SE method provides the technical how-to for building software
- SE tools provide automated or semi-automated support for the process and the methods

## b. A Generic View of SE

- The work associate with SE can be categorized *three generic phase*: **what, how and change**
	- The definition phase focus on *what*
		- what information is to be processed
		- what functions and performance are to be desire
		- what system behavior[^behavior] can be expected
		- what interface are to be established
		- what design constraint exist
		- what validation[^validation] criteria are required to defined a successful system

		*these major tasks will occur in some form:*
		- System or information engineering
		- SW project planning
		- Requirements analysis

	-  The development phase focus on *how*
		- How data are to be structured
		- How function is to be implemented with SW architecture
		- How procedural[^procedural] detail are to be implemented
		- How interfaces are to be characterized
		- How the design will be translated into programming language[^PDL]
		- How testing will be perform
			- white-box testing[^white-box]
			- black-box testing

		*these specific technical task should always occur in*
		- Software design
		- Code generation and Software testing

	- The support (maintenance) phase focus on *change* associate with error correction, adaptation, enhancement & prevention
		**Four** type of change are encounter during the support phase:
		- Correction ---> Corrective maintenance
		- Adaptation ---> Adaptive maintenance
		- Enhancement ---> Perfective maintenance: make software better by adding more feature to serve user need.
		- Prevention ---> Preventive maintenance

	[^behavior]: behavior cause by event.
	[^validation]: validation mean testing.
	[^procedural]: procedural mean algorithms.
	[^PDL]: PDL (Program Design Language) is being use to serve this purpose(to translate design to programming language).
	[^white-box]: white-box testing:
		- top-down testing
		- bottom-up testing (preferred method)
		- sandwich testing
		
# 2.2 Software Life-Cycle
