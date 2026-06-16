# Bi-Directional Jira Sync Workflow (Mural/Miro)

This workflow ensures retrospective outcomes are transformed from static text into tracked engineering issues, preventing action item decay.

## Phase 1: Administrator Configuration
1. Navigate to the App Marketplace of your whiteboard (e.g., Mural).
2. Install the official Jira Cloud or Jira Server integration.
3. Authenticate using an organization-level Jira credential.
4. **Critical Mapping:** Map the specific workspace/board permissions to your designated Jira Project Keys. Failure to restrict this can result in sticky notes being pushed to the wrong backlog.

## Phase 2: Facilitator Execution (During Retro)
1. Identify the finalized, voted-on sticky note cluster.
2. Select the specific sticky note representing the action item.
3. Click the integration menu icon and select `Convert to Issue`.
4. Configure the ticket payload:
   - **Target Project:** Your team's active backlog.
   - **Issue Type:** Task or Story.
   - **Priority:** Assign based on team vote.
5. Execute the push. The sticky note will visually transform to include the Jira issue ID (e.g., `DEV-402`).

## Phase 3: Automation & Verification
- **Status Sync:** Verify the two-way sync by moving the newly created ticket to `In Progress` in Jira. The corresponding card on the whiteboard should immediately reflect this status change.
- **Sprint Roll-over:** At the start of your *next* retrospective, project the Jira board (not the whiteboard) to review the completion status of the previously converted action items.
