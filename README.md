# skillhub

status: rough draft/work in progress

goal is to distill high-value heuristics/mental models/principles for any scenario
can be manual, but ideally is increasingly automated. an external store for autonomous agents
the valuable core of an expert lies in their mental models/heuristics which are honed through much experience
these mental models can be concisely defined and refined
if AI is just advanced pattern recognition, these are the most valuable patterns it can help us distill and hone (and we don't need to wait for it to get started)

minecraft screenshot
https://voyager.minedojo.org/

swyx screenshot/blog post
https://twitter.com/swyx/status/1668679998566461440

https://en.wikipedia.org/wiki/Expert_system
ironically, this may herald a partial reversion to "expert systems", which got much attention early in the early AI boom of the 1950s
yet it's also fitting, there are benefits to expert systems that LLMs can't match. indeed, they complement each other in many areas
from the beginning, if we had an AI, what would be the most valuable thing we could point it at learning? improving its own skills
how are its skills defined? in code, as algorithms
it's no coincidence successful people talk about decision making algorithms
whatever your personal opinions of these people are, the idea comes up repeatedly
https://www.principles.com/principles/be876591-d132-4896-9c44-ea519bad9f1f/
they have a bunch of rules like "5/25" rule

why LLMs unlock expert systems
main limitations to expert systems (https://en.wikipedia.org/wiki/Expert_system)

> Expert systems have superficial knowledge, and a simple task can potentially become computationally expensive.

The language understanding portion of LLMs enables them to describe Since mental models can be described as snippets of code and LLMs can express them as such, these algorithms are no more expensive to run than

> Expert systems require knowledge engineers to input the data, data acquisition is very hard.

LLMs make it easier to distill expert knowledge from raw data/behaviors

> The expert system may choose the most inappropriate method for solving a particular problem.

ML will be used to optimize/"learn"/maintain which methods are most appropriate for solving a given problem and curate set of skills.

> Problems of ethics in the use of any form of AI are very relevant at present.

These problems are real, but they are not unique to AI. They apply to every new technology.

> It is a closed world with specific knowledge, in which there is no deep perception of concepts and their interrelationships until an expert provides them.

See point 2 above.

this may be how the human brain works as well. perhaps LLMs are our frontal lobe and these other components don't need to be built into the same NN (at least for now), and they can instead be separate software modules. would be consistent with the many theories that humans feel they multiple "selves" inside at various times
https://drive.google.com/file/d/1RFxtgLv0q_tKmfzxWG0IOAL8Bre4Id6B/view
https://en.wikipedia.org/wiki/Thinking,_Fast_and_Slow
https://en.wikipedia.org/wiki/Internal_Family_Systems_Model

primitves (TODO)
context: text description, maybe additional structured metadata
role: text description
action: snippet of code

mappings
context to role (which role is appropriate for this context. an index into actions)
context, role to action (which action is most appropriate for a given context. role becomes appended to context?)
action to context (how likely action is to result in certain context)

we see this emerging from prompt engineering already
[cite prompt ex]
also fits in with openai mixture of experts architecture - this can scale to an arbitrary number of experts
https://twitter.com/swyx/status/1671272883379908608

nice properties
it seems obviously safe - easily interpretable/editable. it's just a bunch of text files. no downside to collectively refining the prototypical "best" in role

challenges/risks
do we moderate at all? what if someone puts terrorist or child predator? prob will need some limits for stuff like that, but otherwise let as much be free as possible

appendix
pmarca says early web was built on text - will be curious coincidence if this can be too
something in semantic information theory, not sure what yet though

david deutsch - everything important about the universe can be understood by a human (heuristics)
nassim taleb - world works by distilling heuristics

TODOs

- market research: how much of this exists already in other projects such as langchain. how much will be siloed into separate repos vs. single
- enable agents to run programmatically (act)
- enable agents to provide feedback programmatically (learn)
- tests/simulations
- dev tools to improve ergonomics
- docs

food for thought

- how far can open source community go w/ distilling expert best practices? or will best outcome be achieved by small closed groups of experts?
