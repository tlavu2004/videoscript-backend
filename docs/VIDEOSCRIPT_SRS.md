# VIDEOSCRIPT SOFTWARE REQUIREMENTS SPECIFICATION

## A. Overview

### 1. Product name

VideoScript (AI Short Video Creator) — a platform for creating trend-driven short videos with artificial intelligence.

### 2. Goals

- Help users create short TikTok and YouTube Shorts videos about current topics.
- Use AI technologies such as large language models (LLMs), text-to-speech (TTS), and automated video processing.
- Make content creation easier for general users, students, and multimedia enthusiasts.

### 3. Target users

- People creating short educational, promotional, entertainment, or knowledge-sharing videos.
- Student teams producing examples for communications campaigns.
- Learners experimenting with multimedia AI technologies.

## B. Core MVP features

| ID | Feature                       | Description                                                                |
|----|-------------------------------|----------------------------------------------------------------------------|
| F1 | Trend-based topic suggestions | Suggest topics of current interest from keywords and a trends API.         |
| F2 | Automatic script generation   | Produce an engaging, structured video script.                              |
| F3 | AI voiceover                  | Convert text to speech using TTS.                                          |
| F4 | Automatic video creation      | Combine background images, voiceover, and subtitles into a complete video. |
| F5 | Basic editing                 | Let users add text effects, stickers, and background music.                |
| F6 | Video export                  | Download an MP4 video for sharing or use in a lesson.                      |
| F7 | Created video management      | Store and revisit previously created videos.                               |

## C. Non-functional requirements

- Performance: process a short video (under one minute long) within 60 seconds.
- Extensibility: make it easy to integrate new APIs and advanced features.
- Interface: keep the UI simple and approachable for new users.
- Security: authenticate users and encrypt their information.
- Technical documentation: describe each module to support maintenance and further development.

## D. Main workflow

1. Enter a topic keyword.
2. Generate a script with AI.
3. Generate a voiceover with TTS.
4. Select a suitable background image.
5. Add automatic subtitles.
6. Preview and download the video.

## E. Proposed user interface

- Home page: enter keywords and view trend suggestions.
- Script editor and voice selection page.
- Video preview and basic customization page.
- Dashboard of created videos.

## F. Technology requirements

- Frontend: ReactJS / Next.js + Tailwind CSS (described as already available in the source SRS).
- Backend: Java Spring and Python microservices (Python only for AI-related services).
- AI NLP: propose free third-party models.
- TTS: propose free third-party models.
- Video processing: propose a solution.
- Database: PostgreSQL and MongoDB, assigned to services as appropriate.
- Storage: Cloudinary.

## G. Proposed team responsibilities

- Frontend developer: build the UI and user-facing features (described as already available in the source SRS).
- Backend developer: implement APIs and coordinate AI processing (primary focus).
- AI integrator: connect LLM, TTS, and video rendering services (primary focus).
- Testing and documentation (described as already available in the source SRS).

## H. Evaluation criteria

- An easy-to-use interface.
- Video creation from AI-generated content.
- TTS integration and basic video processing.
- Clear technical documentation and a system diagram.
