function EvaluateOpportunity(job)
{
    score = 0;

    if(job.containsUndefinedProblems)
        score += 100;

    if(job.manager.valuesCuriosity)
        score += 50;

    if(job.requiresLearningNewTechnology)
        score += 40;

    if(job.expectsPoliticalNavigation > TechnicalProblemSolving)
        score -= 80;

    if(job.description == "We've never done this before.")
        return "Let's talk.";

    return score;
}