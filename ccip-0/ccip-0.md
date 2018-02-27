<pre>
  CCIP: 0
  Title: CCIP Purpose and Guidelines
  XCPC Revision and Update: Julian Smith <mailing-dev-list@counterparty.cash>
  Credit: First Author: Devon Weller <dweller@devonweller.com>
  First Publication Date: 2015-10-27
  Status: Proposed
  Type: Counterparty Cash - Development Process Track
  Updated and adapted for XCPCash : 2018-02-24
</pre>

## 1. What is a CCIP?  
**1a.** CCIP stands for Counterparty Cash Improvement Proposal (the "CCIP").  
**1b.** A CCIP is a design document providing information to the Counterparty Cash Assiciation (CCA), or describing a new feature for Counterparty Cash or its processes or environment.  
**1c.** The CCIP should provide a concise technical specification.  
**1d.** Authors MUST outline the feature and a rationale for the feature.  
**1e.** We intend CCIPs to be the primary mechanisms for proposing new features, for collecting community input on an issue, and for documenting the design decisions that have gone into Counterparty Cash.  
**1f.** The CCIP author(s) is responsible for building consensus within the community and documenting dissenting opinions.  
**1g.** Because the CCIPs are maintained as text files in a versioned repository, their revision history is the historical record of the feature proposal.  

## 2. CCIP Types: There are three Types of CCIP.  
**2a.** **(1) Standards Track:**  
**2b.** Standards Track CCIPs Must describe a change which will affect between >1/10th and all Counterparty Cash implementations, such as a change to the network protocol, a change in block or transaction validity rules.  
**2c.** Standards track and any change or addition which affects the interoperability of applications using Counterparty Cash should be considered candidate for elevation to a CCIP.  
**2d.** **(2) Informational:**  
**2e.** All Informational CCIPs describes Counterparty Cash design issues, provides general guidelines or document informal practices maintined within an organisation or indivdidual continbutor practice and add it to the record maintained at GitHub by the Counterparty Cash Assiciation (CCA).  
**2f.** Informational CCIPs do not require to propose a new feature.  
**2g.** Informational CCIPs do not necessarily represent a Counterparty Cash Assiciation (CCA) consensus or recommendation, so users and implementors are free to ignore Informational CCIPs or follow their advice.  
**2h.** **(3) Process:**  
**2i.** A Process CCIP describes a process surrounding Counterparty Cash, or proposes a change to (or an event in) a process.   
**2j.** Process CCIPs are like Standards Track CCIPs but apply to areas other than the Counterparty Cash protocol itself.  
**2k.** They may propose an implementation, but not to Counterparty Cash codebase maintained at GitHub by Counterparty Cash Association (CCA);  
**2l.** They often require community consensus;  
**2m.** Unlike Informational CCIPs, they are more than recommendations, and users are typically not free to ignore them.  
**2n.** Examples include:  
**2o.** 1) Procedures.  
**2p.** 2) Guidelines.  
**2q.** 3) Changes to the decision-making process.  
**2r.** 4) Changes to the tools or environment used in Counterparty Cash development.  
**2s.** 5) Any meta-CCIP is also considered a Process CCIP.  

## 3. CCIP Work Flow  
**3a.** A CCIP editor assigns a CCIP number and changes the status.  
**3b.** Please send all CCIP-related email to the CCIP editor, which is listed under [CIP Editors](#cip-editors) below. Also see [CIP Editor Responsibilities & Workflow](#cip-editor-responsibilities--workflow).  
**3c.** The CCIP process begins with a new idea for Counterparty Cash. It is highly recommended that a single CCIP contain a single key proposal or new idea. Small enhancements or patches often don't need a CCIP and can be injected into the Counterparty Cash development work flow with a patch submission to the Counterparty Cash issue tracker. 
**3d.** The more focused the CCIP, the more successful it tends to be. The CCIP editor reserves the right to reject CCIP proposals if they appear too unfocused or too broad. If in doubt, split your CCIP into several well-focused ones.  
**3e.** Each CCIP must have a champion -- someone who writes the CCIP using the style and format described below, shepherds the discussions in the appropriate forums, and attempts to build community consensus around the idea. The CCIP champion (a.k.a. Author) should first attempt to ascertain whether the idea is CCIP-able. Posting to the [talk.counterparty.cash forums](https://counterpartytalk.org/c/development) or discussing it in the [Counterparty Slack](http://slack.counterparty.io/) is the best way to go about this.  
**3f.** Vetting an idea publicly before going as far as writing a CCIP is meant to save the potential author time. Many ideas have been brought forward for changing Counterparty that have been rejected for various reasons. Asking the Counterparty Cash Assiciation (CCA) first if an idea is original helps prevent too much time being spent on something that is guaranteed to be rejected based on prior discussions (searching the internet does not always do the trick). It also helps to make sure the idea is applicable to the entire community and not just the author. Just because an idea sounds good to the author does not mean it will work for most people in most areas where Counterparty is used.  
**3g.** Once the champion has asked the Counterparty Cash Assiciation (CCA) as to whether an idea has any chance of acceptance, a draft CCIP should be presented on a dedicated thread created by the author in the [talk.counterparty.cash forums' development area](https://talk.counterparty.cash/c/developement). This gives the author a chance to flesh out the draft CCIP and to address initial concerns about the proposal. Discussion should be limited to this forum thread and as much as possible at this time, so as to provide a full record of any debate for all involved parties. Wherever possible, long open-ended discussions should be avoided, and CCIP authors should use their discretion in order to best keep all debate focused, good-natured and material.  
**3h.** Following a discussion, the draft should be submitted to the CCIP editor as a pull request to the [git repository](https://github.com/CounterpartyXCPC/CCIPs). This draft must be written in CCIP style as described below, else it will be closed or otherwise postponed by the CCIP editor until proper formatting rules are followed. All discussion as to the CCIP shall continue either in the comments area of the pull request or in the original forums thread.  
**3i.** If the CCIP editor approves, he will assign the CCIP a number, label it as Standards Track, Informational, or Process, give it status "Draft", and merge it into the [git repository](https://github.com/CounterpartyXCPC/CCIPs). The CCIP editor will not unreasonably deny a CCIP. Reasons for denying CCIP status include duplication of effort, being technically unsound, not providing proper motivation or addressing backwards compatibility, or not in keeping with the Counterparty Cash philosophy (as determined by a majority of the project maintainers as defined below).  
**3j.** The CCIP author may update the draft as necessary in the [git repository](https://github.com/CounterpartyXCPC/CCIPs) via submitting a pull request. Each pull request may host discussion about those specific proposed changes to the Draft, however the CCIP author and editor should stay vigiliant to avoid more general discussion on the CCIP on these subsequent pull requests. Once the pull request is merged, ongoing comments being posted to that pull request should be dissuaded.  
**3k.** Standards Track CCIPs consist of two parts, a design document and a reference implementation. The CCIP should be reviewed and accepted before a reference implementation is begun, unless a reference implementation will aid people in studying the CCIP. Standards Track CCIPs must include an implementation -- in the form of code, a patch, or a URL to same -- before it can be considered "Final".  
**3l.** For a CCIP to be accepted it must meet certain minimum criteria. It must be a clear and complete description of the proposed enhancement. The enhancement must represent a net improvement. The proposed implementation, if applicable, must be solid and must not complicate the protocol unduly.  
**3m.** To be accepted, the CCIP's pull request must be approved ("ACKed") by a majority of Counterparty Cash project maintainers. A Counterparty Cash project maintainer is defined as an individual that has commit access to the (counterparty-lib)[https://github.com/CounterpartyXCPC/counterparty-lib] repository, and has made at least one commit in the last nine month period. If there is only one maintainer, only his or her ACK is necessary.  
**3n.** Once a CCIP has been accepted, its status should formally be set to "Accepted" and its reference implementation must be completed. When the reference implementation is complete and merged into the `master` branch of the relevant Counterparty Cash repositories, the status should be changed to "Final". CCIPs that have no reference implementation (e.g. Process CCIPs) should proceed directly to the "Final" stage upon being ACKed by the project maintainer(s).  
**3o.** A CCIP in "Draft" status can also be assigned a status of "Storage". The CCIP author or editor can assign the CCIP this status when no progress is being made on the CCIP. Once a CCIP is "Storage", the CCIP editor can re-assign it to "Draft" status at-will.  
**3p.** A CCIP can also be "Rejected". Perhaps after all is said and done it was not a good idea. It is still important to have a record of this fact.  
**3q.** CCIPs can also be superseded by a different CCIP, rendering the original obsolete. This is intended for Informational CCIPs, where version 2 of an API can replace version 1.  
**3r.** The possible paths of the status of CCIPs are as follows:  
<img src="https://raw.githubusercontent.com/CounterpartyXCPC/CCIPs/master/ccip-0/ccip-0_workflow_v1.svg?sanitize=true">
**3s.** Some Informational and Process CCIPs may also have a status of "Open" if they are never meant to be completed. E.g. CCIP 1 (this CCIP).  

## 4. What belongs in a successful CCIP?  
**4a.** Each CCIP should have the following parts:  
**4b.** **Preamble** -- RFC 822 style headers containing meta-data about the CCIP, including the CCIP number, a short descriptive title (limited to a maximum of 44 characters), the names, and optionally the contact info for each author, etc.  
**4c.** **Abstract** -- a short (~200 word) description of the technical issue being addressed.  
**4d.** **Copyright/public domain** -- Each CCIP must either be explicitly labelled as placed in the public domain (see this CCIP as an example) or licensed under the Open Publication License.  
**4e.** **Specification** -- The technical specification should describe the syntax and semantics of any new feature. The specification should be detailed enough to allow competing, interoperable implementations for any of the current Counterparty Cash platforms.  
**4f.** **Motivation** -- The motivation is critical for CCIPs that want to change the Counterparty Cash protocol. It should clearly explain why the existing protocol specification is inadequate to address the problem that the CCIP solves. CCIP submissions without sufficient motivation may be rejected outright.  
**4g.** **Rationale** -- The rationale fleshes out the specification by describing what motivated the design and why particular design decisions were made. It should describe alternate designs that were considered and related work, e.g. how the feature is supported in other languages.  
**4h.** The rationale should provide evidence of consensus within the community and discuss important objections or concerns raised during discussion.  
**4i.** **Backwards Compatibility** -- All CCIPs that introduce backwards incompatibilities must include a section describing these incompatibilities and their severity. The CCIP must explain how the author proposes to deal with these incompatibilities. CCIP submissions without a sufficient backwards compatibility treatise may be rejected outright.  
**4j.** **Reference Implementation** -- The reference implementation must be completed before any CCIP is given status "Final", but it need not be completed before the CCIP is accepted. It is better to finish the specification and rationale first and reach consensus on it before writing code.  
**4k.** The final implementation must include test code and documentation appropriate for the Counterparty Cash protocol.  

## 5. CCIP Formats and Templates  
**5a.** CCIPs should be written in markdown format.  
**5b.** Image files should be included in a subdirectory for that CCIP.  

## 6. CCIP Header Preamble  
**6a.** Each CCIP must begin with an RFC 822 style header preamble.  
**6b.** The headers must appear in the following order.  
**6c.** Headers marked with "*" are optional and are described below.  
**6d.** All other headers are required.  

<pre>
  CCIP: <CCIP number>
  Title: <CCIP title>
  Author: <list of authors' real names and optionally, email addresses>
* Workgroup: <url>
  Status: <Draft | Accepted | Rejected | Storage | Closed | Final | Old | WIP>
  Type: <Standards Track | Informational | Process>
  Created: <date created on, in ISO 8601 (yyyy-mm-dd) format>
* Post-History: <dates of postings to the (https://talk.counterparty.cash) forums>
* Requires: <CCIP number>
* Replaces: <CCIP number>
* Superseded-By: <CCIP number>
* Resolution: <url>
</pre>

**6e.** **[CCIP]:** The unique identifyer (number) for the CCIP (once allocated).  
**6f.** **[Title]:** The title of the CCIP (limited to a maximum of 44 characters)  
**6g.** **[Author]:** Lists the names, and optionally the email addresses of the author(s)/owner(s) of the CCIP.  
**6h.** The format of the Author header value must be:  
**6i.** Satoshi Nakamoto <satoshin@gmx.com>  
**6j.** If the email address is included, and just:  
**6k.** "Satoshi Nakamoto" or "Nakamoto, Satoshi" if the address is not given.  
**6l.** If there are multiple authors, each should be on a separate line following the RFC 2822 continuation line conventions.  
**6m.** Note: The Resolution header is required for Standards Track CCIPs only. It contains a URL that should point to an email message, such as a dev-mailing-list server and applicable URI or another web resource where the pronouncement about the CCIP's acceptance is made, such as a dedicated sub project site 'mycoolproject.io' or a Tweet tagging #XCPC AND #CCIP published by one of the identified CCIP authors or the @XCPCash account.  
**6n.** **\*[Workgroup]:** The URL where the CCIP is being discussed while it is in private discussions, usually during the initial draft and development period.  
**6o.** No Workgroup URL is necessary if the CCIP is being discussed privately with the author, or on the Counterparty Cash slack.  
**6p.** **[Status]:** The Staus header specifies the current status of the CCIP.  
**6q.** **[Type]:** The Type header specifies the type of CCIP: Standards Track, Informational, or Process.  
**6r.** **[Created]:** The Created header records the date that the CCIP was assigned a number.  
**6s.** **\*[Post-History]:** The Post-History header is used to record the dates of when new versions of the CCIP are posted to the (https://talk.counterparty.cash) forums.  
**6t.** Both headers should be in yyyy-mm-dd format, e.g. 2001-08-14.  
**6u.** **\*[Requires]:** The Requires header indicates the CCIP number(s) that the CCIP depends on.  
**6v.** **\*[Replaces]:** The Replaces header is optionally used to define the CCIP number(s) the the CCIP replaces.  
**6w.** **\*[Superseded-By]:** The Superseded-By header indicates that a CCIP is rendered obsolete by a later document.  
**6x.** The value is the number of the CCIP that replaces the current document.  
**6y.** The newer CCIP must have a Replaces header containing the number of the CCIP that it rendered obsolete.  
**6z.** **\*[Resolution]:** The Replaces header contains a URL that should point to an email message, such as a dev-mailing-list server and applicable URI or another web resource where the pronouncement about the CCIP's acceptance is made, such as a dedicated sub project site 'mycoolproject.io' or a Tweet tagging #XCPC AND #CCIP published by one of the identified CCIP authors or the @XCPCash account.  

## 7. Auxiliary Files  
**7a.** CCIPs may include auxiliary files such as diagrams. Such files must be named CCIP-XXXX-Y.ext, where "XXXX" is the CCIP number, "Y" is a serial number (starting at 0), and "ext" is replaced by the actual file extension (e.g. "png").  

## 8. Transferring CCIP Ownership  
**8a.** It occasionally becomes necessary to transfer ownership of CCIPs to a new champion. In general, we'd like to retain the original author as a co-author of the transferred CCIP, but that's really up to the original author. A good reason to transfer ownership is because the original author no longer has the time or interest in updating it or following through with the CCIP process, or has fallen off the face of the 'net (i.e. is unreachable or not responding to email). A bad reason to transfer ownership is because you don't agree with the direction of the CCIP. We try to build consensus around a CCIP, but if that's not possible, you can always submit a competing CCIP.   
**8b.** If you are interested in assuming ownership of a CCIP, send a message asking to take over, addressed to both the original author and the CCIP editor. If the original author doesn't respond to email in a timely manner, the CCIP editor will make a unilateral decision (it's not like such decisions can't be reversed :).  

## 9. CCIP Editors  
**9a.** The current CCIP editor(s) is(are) Julian Smith who can be contacted at [julian.smith@blockfreight.com](mailto:julian.smith@blockfreight.com).  
**9b.** There is a Counterparty Cash dev mailing list (the "dev-list") at [mailing-dev-list](http://counterparty.cash/mailman/listinfo/mailing-dev-list_counterparty.cash).  

## 10. CCIP Editor Responsibilities & Workflow  
**10a.** A CCIP editor must belong to the (https://talk.counterparty.cash) forums.  
**10b.** All CCIP related correspondence should be sent (or CC'd) to the dev-list.  

## 11. CCIP Editor(s) role(s) - each new CCIP that comes into an editor does the following:  
**11a.** Read each CCIP to check if it is ready: sound and complete.  
**11b.** The ideas must make technical sense, even if they don't seem likely to be accepted.  
**11c.** The title should accurately describe the content.  
**11d.** Edit the CCIP for language (spelling, grammar, sentence structure, etc.), markup (for reST CCIPs), code style.  
**11e.** If the CCIP isn't ready, the editor(s) will send it back to the author for revision(s), with specific instruction(s).  
**11f.** Once the CCIP is ready for the repository, the CCIP editor will:  
**11g.** Assign a CCIP number (almost always just the next available number, but sometimes it's a special/joke number, like 666, 420 or 3141).  
**11h.** Add the CCIP to the [CounterpartyXCPC/CCIPs](https://github.com/CounterpartyXCPC/CCIPs) repository on GitHub.  
**11i.** List the CCIP in [README.md](https://github.com/CounterpartyXCPC/CCIPs/blob/master/README.md)  
**11j.** Send email back to the CCIP author with next steps (post to (https://talk.counterparty.cash) forums).  
**11k.** Many CCIPs are written and maintained by developers with write access to the Counterparty Cash codebase.  
**11l.** The CCIP editors monitor CCIP changes, and correct any structure, grammar, spelling, or markup mistakes we see.  
**11m.** The editors don't pass judgement on CCIPs.  
**11n.** We merely do the administrative & editorial part.  
**11o.** Except for times when there's relatively low volume.  

## 12. History  
**12a.** This document was derived heavily from Bitcoin's [BIP-0001](https://github.com/bitcoin/bips/blob/master/bip-0001.mediawiki), which was derived heavily from Python's PEP-0001.  
**12b.** In many places text was simply copied and modified.  
**12c.** PEP-0001 text was written by Barry Warsaw, Jeremy Hylton, and David Goodger.  
**12d.** They are not responsible for its use in the Counterparty Cash Improvement Process, and should not be bothered with technical questions specific to Counterparty Cash or the CCIP process.  
**12e.** Please direct all comments to the [talk.counterparty.cash forums](https://counterpartytalk.org/c/development) or the dev-list.  
**12f.** This was then here updated in Feb 2018 for Counterparty Cash Association (CCA) by [Julian Smith](mailto:julian.smith@blockfreight.com)  