---
layout: posts
title: Live Coding With a Screen Reader
tags: SuperCollider NVDA
---

<p>After 10 weeks of study, troubleshooting, tears, and luck, I was finally able to use my screen reader in a live coding performance!</p>

<section class="center" id="performance">
<iframe width="560" height="315" src="https://www.youtube.com/embed/ZWFjWbyrl0g?si=jPRZHgPaDTzYVcV-" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</section>

<h2>Designing for My Own Disability</h2>

<p>This performance was developed as part of my MSc in Sound Design and Audiovisual Practice at the University of Glasgow in response to barriers I encountered using industry-standard sound design tools with my screen reader.</p>

<p>Though I am sighted, I have a disability that prevents me from using a mouse, reading, and looking at a screen for long periods of time without getting fatigued. This barrier means that many artistic and technical decisions that go into an independent project like this one are for me driven more by which tools are accessible than which tools are considered best suited for the job. My primary criterion for which software to use for this performance in particular was how compatible the interface would be with NonVisual Desktop Access (<a href="nvaccess.org">NVDA</a>), my preferred screen reader on Windows.</p>

<p>REAPER is fully accessible for screen reader users thanks to the <a href="https://osara.reaperaccessibility.com/">OSARA extension</a> and tools such as the Actions List, which makes it my preferred DAW. For a live performance, however, software like Max MSP that would normally be suited to the task are not built for keyboard-only navigation and are much more difficult for me to navigate. While there are work-arounds like <a href="https://addons.nvda-project.org/addons/goldenCursor.en.html">the Golden Cursor add-on for NVDA</a> that I can use to work in moderately inaccessible software, setting this up is often too slow to be practical on a tight deadline.</p>

<p>It was this constraint that convinced me to finally sit down and learn the basics of live coding in SuperCollider and then try to adapt the program so I could use my screen reader during the performance without distracting either myself or my audience from the core sounds I wished to highlight.</p>

<h2>Personifying Mark</h2>

<p>The voice of "Mark the Screenreader" is a slow-paced, mid-pitched version of the "Microsoft Mark" voice on the Windows OneCore Voices synthesizer that comes with NVDA. Mark's comments and commands heard throughout the performance are pre-written in a SuperCollider file I navigated through during the performance using keyboard shortcuts. Designing for this kind of navigation meant that code placement and white space became much more important for me to consider than a live coder with a visual display. I stuck to a single file for the entire performance, reserving the top of the editor for a note about a glitch I was unable to address by the day of the performance, the end of the script for the most basic playback option that I knew I would have to find often and quickly, and the middle of the document for setup code and less frequently used functions.</p>

<p>I used NVDA's speech dictionary, which is normally used to correct the occasional mispronunciation or misidentification of a particular word in context, to translate long lines of code into brief descriptions of what I was using that line of code to do:</p>

<img src="/docs/assets/nvda_sc.png" 
        alt="screenshot of SuperCollider code on left and their translations in NVDA's default dictionary on the right"
        height=500px>

<p>While slow, I found this "translation" to be the only way I could monitor my code and my looped sounds onstage at the same time, while still allowing the audience to "look under the hood" and attempt to understand what I was doing as they would be able to in a conventional live coding performance.

<p>Surprisingly, this decision also had the unintended consequence of creating the illusion of "Mark" being a coperformer, with audience members commenting later that it was "hard to tell who was in charge" and that it almost seemed as if I was "the screen reader's hands".</p>

<h2>More Than an Afterthought</h2>

<p>Encountering unintended benefits when designing with accessibility in mind from the beginning is a well known phenomenon in architecture and user interface design, often referred to as the <a href="https://web.archive.org/web/20181220090501/http://www.accessiblesociety.org/topics/technology/eleccurbcut.htm">curb cut effect</a>. The more I work with accessibility and sound design, the more potential I see for surprising artistic discovery arising naturally from embedding disabled perspectives in teams beyond standard user interface or accessibility design roles. This inclusion of disabled designers in a wide variety of teams at all stages of development is the kind of work environment I want to facilitate throughout my career as a technical sound designer.</p>

<h4>Acknowledgements</h4>

<p>Thank you to <a href="https://www.gla.ac.uk/schools/cca/staff/nicolasfells/">Professor Nick Fells</a> for an excellent crash course in SuperCollider and his generous donation of the SynthDefs used in recording and playback.</p>
