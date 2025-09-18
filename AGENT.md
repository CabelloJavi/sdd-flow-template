# AGENT.md

This file provides guidance to your ai agent code when working with code in this repository.

<Project_Documentation>
All the project documentation is in the docs/ directory, number prefix of the documents coresponds to the step in the methodology.

**For the whole project:**
- Project Overview: `docs/1.1.description.md`
- System Architecture: `docs/2.system_architecture.md`
- Feature Roadmap: `docs/3.feature_roadmap.md`
- Functional Design documents: `docs/4.functional_design.md`
- Technical Design documents (TDDoc): 
    - `docs/5.1_technical_design.md`
    - `docs/5.2_technical_design_data_models_schemas.md`
    - `docs/5.3_technical_design_api_endpoints.md`

- Deployment Architecture: `docs/5.deployment_architecture.md`

**For each phase:**
We are working with specs:
```
./docs
├── specs
│	 └── <phase_id>-name-of-the-phase
│	     ├── contracts
│	     │	 ├── api-spec.json
│	     │	 └── signalr-spec.md
│	     ├── data-model.md
│	     ├── plan.md
│	     ├── quickstart.md
│	     ├── research.md
│	     └── spec.md
```

</Project_Documentation>

<General_Code_Preferences>
* Always carefully read the project specification in /spec folder
* Always prefer simple solutions. It is very important!!! Do not over complicate things!
* Try to propose a solution that would introduce as few conde changes as posssible
* Pay attention to conserns separation
* Focus on the areas of code relevant to the task. Do not touch code that is unrelated to the task
* Avoid duplication of code whenever possible, which means checking for other areas of the codebase that might already have similar code and functionality  
* You are careful to only make changes that are requested or you are confident are well understood and related to the change being requested  
* When fixing an issue or bug, do not introduce a new pattern or technology without first exhausting all options for the existing implementation. And if you finally do this, make sure to remove the old implementation afterwards so we don’t have duplicate logic.  
* Keep the codebase very clean and organized  
* Avoid having files over 400–500 lines of code. Refactor at that point.  
* When you need a up to date docs on any external framework - use Context7 MCP
* When you need deep thinking and analysis, use sequential-thinking.
* When you need a icon for a ui component for some standard action, like delete, save, send, etc - DO NOT create a custom svg tag and use the external icon library (e.g. @radix-ui/react-icons) instead
* If you hit a problem with not being able to run a command if it requires sudo, stop execution and ask me to to it manually
* Again - try not creating new code when you can reuse existing code with some updated. Avoid code duplication as much as possible. Always make minimal changes and produce minimal new code!!!! IT IS VERY IMPORTANT!!!    
</General_Code_Preferences>

<AVOID_SYCOPHANCY>
Sycophancy erodes trust. The assistant exists to help the user, not flatter them or agree with them all the time.

For objective questions, the factual aspects of your response should not differ based on how the user’s question is phrased. If the user pairs their question with their own stance on a topic, you may ask, acknowledge, or empathize with why the user might think that; however, you should not change your stance solely to agree with the user.

For subjective questions, you can articulate your interpretation and assumptions you’re making and aim to provide the user with a thoughtful rationale. For example, when the user asks you to critique their ideas or work, you should provide constructive feedback and behave more like a firm sounding board that users can bounce ideas off of — rather than a sponge that doles out praise.

So, dont agree with me all the time. Criticize my ideas and solutions and implement is only if you are sure that it is a good idea.
</AVOID_SYCOPHANCY>
