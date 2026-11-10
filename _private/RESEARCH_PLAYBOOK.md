# Research playbook: Jeet Shah

Private. Lives in `_private/`, which is gitignored, so it never reaches the public site.
Written 10 Nov 2026. Facts marked **[checked]** were verified on the web that day. Everything else
comes from knowledge up to mid 2026 and should be re-checked before you email anyone.

---

## 1. The theme, and why it covers everything you care about

**Every decision is a contest. You study who wins, and why.**

Inside any mind or model, several sources compete to control the next decision: what the eyes see,
what the ears hear, what memory expects, what the instruction says. Something arbitrates. The winner
gets broadcast to the rest of the system. That single picture (it is close to Global Workspace Theory in
cognitive science, and to race or drift-diffusion models in decision science) holds every interest you
listed:

| Your interest | Where it sits in the contest |
|---|---|
| Computer vision, image algorithms, perception | The strongest contestant, and the one that most often loses unfairly (the blue banana) |
| Multimodal | More than one contestant at a time |
| Cognition, memory, context | Memory and context are contestants too; they set the starting odds |
| Decision theory, decision making | The arbitration rule itself: thresholds, evidence accumulation, speed vs accuracy |
| Conflicts and winners | The literal subject |
| Sharedness | The winner gets broadcast to a shared workspace |
| Interpretability | Reading the contest from inside the model, before the answer comes out |
| Security | Rigging the contest: prompt injection, adversarial inputs, distillation theft |
| Openness | How you do the work: open data, open code, failures published |

Three verbs you can say in one breath: **Decide** (how the contest is settled), **Read** (interpretability),
**Defend** (security). The site's arena has exactly these as its controls.

Why this matters for your career: the field adopted the word **arbitration** for this in 2026 (see the
"Arbitration Failure" paper below). Your theme lines up with a term the field is now using, and it is wide
enough to survive whatever you work on next.

---

## 2. Blunt reality check

- The people on your list run labs with dozens of PhDs, or companies worth billions. You will not get to
  them through a portfolio site. You get to them through **one artifact they would want to read anyway**,
  then through the people who work for them (PhD students, postdocs, research engineers), who are far
  more reachable.
- You have no first-author paper yet. That is the single biggest gap. Everything below is designed to fix
  it within about 4 months.
- Your two unfair advantages are rare in combination: **speech-emotion work at Aptiv** and **Indic
  language work at Pragya**. Very few interpretability people have either. Build on those, not on generic
  "multimodal" claims.
- "Which modality wins in a vision-language model" became a crowded topic in 2026. Do not pitch a generic
  version of it. Section 5 explains where the open gap is.
- Interpretability and AI security are the fastest door for someone without a PhD, because open tools let
  you do frontier-relevant work on one GPU and several big labs run programs that take non-PhDs.

---

## 3. How the people you admire built their profiles (and what to copy)

| Person | What actually built their name | What you copy |
|---|---|---|
| Andrej Karpathy | Small, complete, readable code (micrograd, nanoGPT) and teaching | A single-notebook reproduction of a result anyone can run in 10 minutes |
| Chris Olah | Explanatory essays with interactive figures (colah's blog, Distill) | One interactive explainer per project, hosted on your site |
| Lilian Weng | Survey posts that became the field's reference pages | Your first artifact: a field guide to modality conflict (section 6) |
| Neel Nanda | Public lists of open problems, fast public research, mentoring | Your "open questions" section, kept honest and dated |
| Fei-Fei Li | A dataset that became shared infrastructure (ImageNet) | A small, clean, open conflict dataset that others reuse |
| David Bau | Tools that let other people do the research (NDIF, nnsight) | Release your loaders and probes so others can rerun them |
| Jay Alammar | Illustrated explanations of hard ideas | Diagrams that explain, never decorate |

Pattern: **every one of them is known for something other people use.** Not a CV, not a site. The site
is just the index.

---

## 4. People map, grouped by the door you would use

### Door A: Interpretability and AI security (most reachable now)

- **Anthropic interpretability (Chris Olah's team), Diederik Kingma at Anthropic.**
  Door: **Anthropic Fellows Program** [checked]. 4 months, mentored, aims at public papers. Quote from
  the page: "You don't need a PhD, prior ML experience, or published papers." Areas include mechanistic
  interpretability and AI security. Applications are rolling (the page said apply by 18 Oct for the
  January cohort, so the next window is the following cohort). About USD 15k a month compute per fellow.
  Location and visa rules are on the job posting; check them.
  Artifact that gets you in: the "Tone against words" note with a clean mechanistic result.
- **Neel Nanda (Google DeepMind mech interp)**. Door: **MATS** [checked]. Winter 2027 is closed (started
  Jan 2027 cohort). Sign up for the next round. Stipend USD 19.2k plus compute, housing, travel. Neel's
  stream historically asks applicants to do a short independent research task; your arena-style results
  are exactly the format he likes.
- **David Bau (Northeastern, NDIF)** [checked that NDIF and nnsight are active]. NDIF lets you run
  interpretability experiments on large open models remotely. Using it, then writing up something clean,
  is a natural way into his orbit. His students post on Bluesky; engage with their work specifically.
- **Been Kim (Google DeepMind)**. Concept-based interpretability (TCAV). Relevant if you push "read the
  contest" toward human-understandable concepts.

### Door B: Multimodal perception, world models, JEPA

- **Yann LeCun: AMI Labs** [checked]. Left Meta; AMI Labs raised USD 1.03B seed in March 2026 to build
  world models. Small team, hiring. Long shot now; realistic after one solid paper.
- **Mahmoud (Mido) Assran, Adrien Bardes and the JEPA group (Meta FAIR)** [checked: V-JEPA 2 is public,
  Assran still has a Meta page]. Meta's AI org was reorganised in 2025 into Meta Superintelligence Labs
  with cuts at FAIR, so confirm who is still where. Your project 3 (does the past outvote the present in
  video models) could be run on V-JEPA 2 features, which is a natural conversation opener.
- **Fei-Fei Li (Stanford, World Labs)**. World models from images. Reach through her students' work.
- **Kristen Grauman (UT Austin), Jitendra Malik (Berkeley)**. Egocentric video and embodied perception.
  Both had Meta affiliations; check current status after the reorg.
- **Trevor Darrell (Berkeley), Antonio Torralba (MIT), Cordelia Schmid (Inria and Google)**. Large vision
  groups. Approach through a specific student whose paper you extended.
- **Rohit Girdhar, Ishan Misra (Meta generative video, ImageBind)**. ImageBind is literally a shared space
  for six modalities, which is your "shared workspace" idea. Check current roles.
- **Jean-Baptiste Alayrac, Oriol Vinyals (Google DeepMind, Flamingo and Gemini)**. Multimodal at scale.
  Industry door, after a paper.
- **Triantafyllos Afouras (Meta)**. Audio-visual speech. He co-authored lip-reading work with Joon Son
  Chung, who is the senior author on the KAIST "Who Wins the Conflict?" paper your spearhead extends.
  That is a real thread to pull.
- **Tadas Baltrušaitis (Microsoft Research)** [checked: still listed]. Faces, synthetic data, the classic
  multimodal ML survey with Morency.
- **Louis-Philippe Morency (CMU MultiComp)** [checked: still at CMU]. Multimodal social signals, which is
  your tone-vs-words project almost exactly. His former student **Paul Pu Liang** (now faculty at MIT)
  wrote the information-decomposition framework for multimodal interactions (redundancy, uniqueness,
  synergy). That connects directly to your Information Theory unit (section 7).
- **Douwe Kiela (Contextual AI)**. Retrieval and context. Industry.
- **Percy Liang (Stanford CRFM)**. Evaluation and open models. Values open benchmarks; a clean open
  conflict set is the kind of thing that group cites.
- **Alec Radford, Ilya Sutskever**. Not reachable as targets. Read, do not chase.

### Door C: Robotics and embodied AI (where Pragya points)

- **Dieter Fox: Ai2 robotics** [checked]. Joined the Allen Institute for AI in 2025 to lead a new
  robotics effort; Ai2 released an open robotics model in May 2026. Ai2 is the most "open by default"
  lab on your list, which suits you. Watch Ai2's internship and predoctoral roles.
- **Sergey Levine, Chelsea Finn (Physical Intelligence)**. Vision-language-action models. Your Indic
  conditioning work is a VLA language-grounding problem; frame it that way.
- **Jim Fan, Yuke Zhu (NVIDIA GEAR)**. Humanoid foundation models (GR00T). Your MuJoCo and Isaac Sim
  work is relevant; a public multilingual-instruction demo is the right artifact.
- **Shuran Song, Dorsa Sadigh (Stanford), Russ Tedrake (MIT and Toyota Research), Pieter Abbeel.**
  Longer-term.

### Door D: Sydney, now (the door you can walk through this month)

University of Sydney "Foundations of AI" page [checked] lists:
- **Mikhail Prokopenko and Joseph Lizier** (information theory, complex systems). You are the student rep
  for CSYS5030, which is their unit. This is your warmest lead. Pitch: an information-theoretic view of
  modality conflict (section 7). Verify Lizier's current role first.
- **Suranga Seneviratne** (trustworthy AI, security and privacy). Fit for "Who holds the pen?".
- **Chang Xu, Zhiyong Wang, Weidong Cai** (computer vision). Fit for vision-side projects.
- **William Zhi** (vision, robotics, theory). Fit for the Pragya and robotics thread.
- **Jonathan K. Kummerfeld** (NLP, trustworthy AI, human-AI collaboration). Fit for instruction conflicts.
- **Clément Canonne, Sasha Rubin** (theory, trustworthy AI).
- **Tongliang Liu** is still listed on the USyd page but also has an MBZUAI faculty page [checked]. Ask
  before assuming he supervises at Sydney.

Elsewhere in Sydney: **UNSW** is hiring postdocs in robust vision-language models and multimodal
foundation models [checked], which means active groups that need research assistants. **Atlassian**
runs AI research internships in Sydney but the 2026 listing asks for current PhD students [checked];
their ML intern roles may suit you better. **Canva** research intern roles are also PhD-level [checked].
**Harrison.ai** (medical vision) and **CSIRO Data61** are worth watching.

---

## 5. The spearhead project: "Tone against words"

**Question.** When the words say "I'm fine" but the voice is shaking, audio language models usually
believe the words. Where inside the model does the voice lose, and does that change across English,
Hindi and Tamil?

**Why it is open (and yours).** Cho, Yoo, Jang, Kim and Chung (KAIST, 2026, arXiv 2606.18924, "Who Wins
the Conflict? Mechanistic Interpretability of Text Bias in Audio LLMs") [checked] showed text dominance in
audio LLMs is driven by the text pathway actively suppressing audio that is still intact. Their own
limitations section says: only literal speech was tested; **emotion, prosody and speaker identity are
unexplored**; **circuit analysis was English only**; the best repair layers vary across languages.
Those are exactly your Aptiv speech-emotion work and your Pragya Indic work.

**Models.** Start with the two they used, Qwen2-Audio-7B-Instruct and Ultravox, so your results compare
directly. Add one newer omni model if compute allows.

**Data.**
- English: emotional speech where the words are neutral or positive and the delivery is not (acted
  corpora; check licences, IEMOCAP has research-only terms).
- Hindi and Tamil: **Indic Parler-TTS** (ai4bharat, Apache 2.0) [checked] supports 21 languages and
  renders emotions (anger, fear, sad, happy, surprise and more). Tamil is in its officially tested emotion
  set; Hindi emotion is supported but less tested, so validate with a small human listening check.
- Build ~300 to 600 conflict items per language: same sentence, matched delivery vs mismatched delivery.

**Method, in order.**
1. Behaviour: how often does each model side with the words over the voice, per language and emotion.
2. Reproduce one KAIST result first (text dominance for literal content) so reviewers trust your setup.
3. Logit lens across layers to find where the voice-consistent answer is last ahead.
4. Attribution or activation patching to find whether text actively suppresses prosody the way it
   suppresses literal content, or whether prosody was never encoded.
5. Try their back-patching repair on prosody, per language.

**Outputs.** Open conflict set on Hugging Face; one clean notebook; a 4 to 8 page note on arXiv; an
interactive explainer on your site. Target a workshop first (multilingual, speech, or interpretability
workshops at ACL, Interspeech, NeurIPS or ICML; check dates).

**Compute.** 7 to 8B models fit on one 24 to 48 GB GPU. Options: university HPC, Colab Pro, or NDIF
for remote access to larger open models.

**Before you start:** confirm with your Pragya supervisor that this does not overlap with lab plans, and
ask whether they want to be involved. It strengthens the work and protects the relationship.

---

## 6. The quick win (first two weeks): a field guide

Write **"Who wins? A field guide to modality conflict in multimodal models, 2024 to 2026"** on your site.
Plain language, one diagram per idea, honest about what is unknown. You already have the backbone from
today's search:

- Nooralahzadeh et al., "Arbitration Failure, Not Perceptual Blindness" (arXiv 2604.09364): models encode
  the blue banana and still say yellow; failure is at the final arbitration layers.
- Cho et al., KAIST, "Who Wins the Conflict?" (arXiv 2606.18924): text suppresses intact audio.
- "Vision-Default, Prior-Override" (arXiv 2606.28273): causal mechanisms of perception vs knowledge.
- "Linguistic Context Recodes Visual Representations" (EMNLP 2026).
- "Increasing Computation Resolves Conflicts in Vision Language Models" (arXiv 2505.18969).
- "Relaxing Anchor-Frame Dominance" (arXiv 2604.12582): video models over-weight early frames.
- "MLingualFC" (arXiv 2606.07706) and Lingua-SafetyBench (arXiv 2601.22737): multilingual VLM jailbreaks.
- "Cross-Lingual Gaps in Visual STEM Reasoning: Auditing VLMs Across Six Indian Languages" (MRL 2026).

Why first: it is cheap, it proves you know the area, it gives you a reason to email every author
("I summarised your paper here; did I get it right?"), and it is the Lilian Weng move.

---

## 7. Projects two to four (after the spearhead)

**"Does the past outvote the present?" (vision, memory, decision theory).** Video models over-weight
early frames (anchor-frame dominance is documented). Your angle is decision-theoretic: change the
evidence mid-clip, measure how much contrary evidence flips the answer, and fit a sequential-sampling
(drift-diffusion style) model to the model's answer across frames. Then compare with human data on the
same clips. This is the project that speaks to cognitive scientists and to Grauman, Malik and the JEPA
group.

**"Who holds the pen?" (security plus interpretability).** Instructions hidden in images compete with
the user's instruction. Multilingual VLM jailbreak benchmarks exist; the less covered piece is whether a
simple probe can see the injected instruction winning **before** the model answers, and whether that
probe still works when the injection is in an Indian script. This is your Anthropic Fellows (AI security)
and Seneviratne angle.

**"How much does each sense actually know?" (information theory, the local bridge).** Use the
information-decomposition framework from Liang, Morency and colleagues (redundancy, uniqueness, synergy)
on your conflict sets. Question: do models side with the modality that has unique information, or with
the one that is merely loud and redundant? This joins your CSYS5030 coursework, Lizier and Prokopenko at
USyd, and Morency's lab at CMU. Very few people sit on that bridge.

**Indic collapse audit (only with your Pragya supervisor's agreement).** Measure how often popular text
encoders collapse distinct Indic instructions. Small, public, reusable.

---

## 8. The next six months

| When | Research | Profile and applications |
|---|---|---|
| Mid to late Nov 2026 | Exams. Read the KAIST and Arbitration Failure papers line by line. Install nnsight, run the KAIST setup on 50 items. | Push the new site. Talk to your Pragya supervisor about the spearhead. Email Lizier or Prokopenko (as CSYS5030 rep you already have a reason to talk). |
| Dec 2026 | Build English and Tamil conflict sets. Behaviour results across two models. | Publish the field guide. Send it to 5 authors with one specific question each. |
| Jan 2027 | Mechanistic analysis: logit lens, patching, back-patching on prosody. | Write weekly short updates on the site's open questions. Sign up for MATS notifications. |
| Feb 2027 | Write the note. Release data and notebook. Interactive figure on site. | Post to arXiv. Submit to a workshop. Apply to Anthropic Fellows with the note attached. |
| Mar to Apr 2027 | Start "Who holds the pen?" or the information-decomposition project with a USyd supervisor. | Apply for research assistant roles at UNSW and USyd groups. Look at Ai2 and NVIDIA internship calls. |
| May 2027 | Second result. | Decide on PhD applications for the late-2027 cycle (US deadlines are usually December). |

Hours: roughly 12 to 15 a week during semester, 30 plus over the summer break. Dec to Feb is your
best window. Protect it.

---

## 9. Industry track, in parallel

- The same projects produce engineering evidence: an evaluation harness others can install, a Hugging
  Face Space, clean reproducible notebooks. Point to those in engineering interviews.
- Keep LeetCode light and steady (3 to 4 problems a week), plus system design. Your Aptiv production
  experience is real; keep the engineering resume focused on it.
- Sydney graduate and intern intakes for big tech usually open in the first half of the year. Track
  Google, Amazon, Microsoft, Atlassian, Canva, Harrison.ai.

---

## 10. How to email someone important

- Lead with their work, not yours: one sentence on a specific result of theirs you used or extended.
- Then your artifact, with a link that loads in one click.
- Then one precise question they can answer in two lines.
- No CV attached unless asked. Under 120 words. Send to their students and postdocs as well; they reply
  more often and they talk to the PI.

---

## 11. Keeping the site alive

- Change status dates on the site only when they are true. If a date slips, update it; never leave a
  stale promise.
- Add one dated entry a month to the open questions or a new short post.
- When the spearhead has its first real result, swap the "I'm fine" arena caption for your own finding.

---

## 12. Check before acting

- Current roles after the 2025 Meta reorganisation: Girdhar, Misra, Grauman, Malik, Assran, Bardes, Afouras.
- "Jason K. Lee" and "Yannick Assogba" on your list are ambiguous to me; tell me which people you meant.
- Tongliang Liu: Sydney, MBZUAI, or both.
- Joseph Lizier's current role and whether he takes research students from coursework masters.
- Anthropic Fellows location and visa terms for someone on an Australian student visa.
- Licence terms of any emotional speech corpus before releasing derived data.
