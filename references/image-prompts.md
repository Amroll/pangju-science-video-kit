# 封面、视频关键帧与可选原理图模板

花括号变量须在调用前替换。以下模板为本技能自身的生图流程，不调用任何其他风格技能。用户指定内容优先。

## 1. 封面

输入顺序：身份三视图、随包封面风格范例。范例中的具体知识点不是本期内容。

```text
Create ONE finished Chinese science short-video cover, {portrait 9:16 OR landscape 16:9}, opaque background.
Image 1 is the sole CAT IDENTITY reference. Image 2 is only the 2D COMIC STYLE / TYPOGRAPHY reference. Replace its old topic, text, props and situational expression with this episode's content.
Topic: {topic}. Verified answer: {answer}.

The SAME extremely chubby orange tabby, broad white muzzle and bib, white paws, orange stripes with forehead M, green eyes, pink-brown nose, small triangular ears, thick ringed tail. Strong expressive hand-drawn 2D anime, bold ink outlines, cel shading, stylized furry detail. Cover rendering is 2D; preserve character identity from the 3D reference.
Expression: {topic_relevant_reaction}. Pose: {pose}. Main prop: {prop_in_correct_state}. Exactly two ears, one iris and one pupil per eye; no third triangular ear-shaped tuft. No human hands, extra limbs or extra tail.

Warm pale-yellow comic-paper background, dark-navy massive Chinese lettering, thick cream outlines, red-orange highlighted key word, one red conclusion badge. Controlled edge speed lines and halftone dots. Cat eyes and title readable at thumbnail size; generous margins.
Layout: {vertical: small label above, two-line title in upper part, cat in middle, conclusion badge below; OR horizontal: title on left, cat on right, conclusion badge near bottom, balanced with prop}.

Render ONLY these exact Chinese strings:
Series label: “胖橘小科普”
Title first line: “{topic_title}”
Title second line: “{question_title}”
Conclusion badge: “{short_accurate_answer}”
{optional exact small footer text, otherwise no footer}

No unrequested text, watermark, app UI or other characters. Do not reuse soot, smoke, alcohol lamp or explosion unless this episode requires them. One finished cover, not a contact sheet.
```

## 2. 视频首帧

仅以三视图锁定角色；不要把漫画封面用作视频画风参考。默认原三视图的3D质感。整片首帧必须显出所选异常、对比或行动受阻；段间首帧则承接已成立的状态，不重新制造开场钩子。分段生图时将时间标签改为“第i段局部0秒/对应全片S秒”，按本段实际场景填写。

```text
Create the OPENING KEYFRAME for {whole video or segment number}, at {overall time 0 or segment-local 0 / overall S}, {aspect_ratio}, opaque full scene. Overall edited runtime is {T} seconds; each generated segment is 10 seconds. Follow the exact state assigned to this frame.
The supplied three-view cat image is the strict identity, proportions, fur and 3D-rendering reference. Render ONE cat in ONE shot, not three views.
Preserve the exact extraordinarily fat orange tabby, broad cheeks, white muzzle/chest, white paws, green eyes, forehead M and stripes, pink-brown nose, exactly two short ears, thick ringed tail. Same recognizable face, no costume or accessories. Each eye has one intact iris and pupil, with coordinated gaze. Fluffy fur must not create a third triangular ear.
This cat is an excitable, experiment-obsessed science enthusiast. Show the specific storyboard action and its emotional cause: {active pose, gaze target, visible cause of excitement}. Do not freeze the reference's half-lidded expression or replace action with an angry face; do not add a scientist costume.
High-quality warm 3D animation rendering matching the reference, not the 2D comic cover style.

Scene: {scene}. Camera/framing: {camera}. Layout adapted to {aspect_ratio}: {positions}.
Exact opening state from storyboard: {cat_pose_and_expression_and_action_phase}; {diagram_or_prop_state_and_count}.
Instantly visible hook for the overall first frame, or carried state for later segments: {specific anomaly, comparison, blocked goal, or ongoing causal state}. Gaze target: {object}; contact/action point: {position}. Make the focal difference readable without captions; use one clear focus, not several competing diagrams. Do not default to a seated presenter waiting to speak.
For an opening based on action or contrast, show the specific physical evidence assigned to this instant: {deformation, displacement, contact, motion phase or comparative state}. A strained facial expression alone is not evidence of the object's behavior. Depict only this instant; later contrasting results belong in their planned shots, not an unrequested split-screen.
Choose composition and scene from the storyboard's action and scientific focus; a classroom is optional, not mandatory. Any hazardous process exists only as a clearly separate teaching illustration, never a live hazard beside the cat.
Framing must keep the important action, contact point and expression readable; an intentional close-up need not show the whole body. Correct four-limb feline anatomy. Hands remain paws.
Leave space for postproduction captions. No text, subtitles, watermark, speech bubble or cover headline. Soft consistent lighting, clean uncluttered background. Show exactly the storyboard's opening state; a result-first hook is allowed when explicitly planned, but do not introduce unplanned later states.
```

## 3. 视频尾帧

输入顺序：本段实际首帧、身份三视图。首帧是编辑目标；三视图是身份辅助。精确列出“什么动作经过什么过程造成了什么可见变化”，不仅写“生成尾帧”或只换表情。默认尾帧对应本段局部10秒；末段保留R<10秒时，此终态必须从R秒前已成立，并延续到10秒供裁剪。提示词的时间标签按分段表填写，不把每一段都当成全片0—T。

```text
Edit image 1 into the MATCHING END KEYFRAME for {whole video at T or segment number at local 10 seconds}. Image 2 is the strict supporting cat identity reference. If this segment retains only R seconds, the final state must already be reached by R and continue through local 10; do not introduce a later result that would be cut out.
For a full retained 10-second segment, this is an instantaneous frame reached at the end, not a pose to hold for the final seconds. Motion phase at the boundary: {readable ongoing movement or brief completed reaction}. For a shared boundary, the next segment continues with {next action phase}. Do not introduce blur that hides anatomy or the scientific result.
Preserve image 1's {aspect_ratio} canvas, 3D rendering, cat identity, anatomical proportions, fur and markings. Preserve environment, camera, lighting and prop design wherever the storyboard does not explicitly change them. A planned close-up or scene change is allowed; do not force the opening composition onto a different ending shot.
Only the following storyboard-driven changes are permitted:
1. Cat final pose and expression: {final_pose}. Specify exactly which paw moves and which remains planted. When a paw lifts, remove it from its old ground position. No extra limb, human hand or fingers.
2. Teaching diagram / prop final state: {precise_final_state}. Keep object count {count}. Show the completed scientific result accurately. The visible difference from the start is {specific state change}, caused in the storyboard by {action and intermediate mechanism}; do not invent a result, imply an unshown cause, or replace the state change with a facial reaction.
3. Camera/framing/scene changes: {only explicitly planned changes, otherwise preserve the opening camera and scene}. Specify the new screen positions if the angle changes; keep object relationships and the causal outcome consistent.
Objects not involved in planned changes stay in their established scene positions. Maintain one cat, exactly two ears and one tail, correct single irises and pupils, and coordinated gaze. No subtitles, labels, cover graphics or watermark. Preserve caption breathing space. A single final animation frame, not a montage.
```

## 4. 按需生成原理参考图

仅当本期剖面/放大机制复杂、现有首尾图无法约束关键结构时使用。以本期实际道具图为结构参考，按[视觉叙事规则第3节](visual-storytelling.md#3-让原因经过画面到达结果)先写清对应关系，再生成一张供相关镜头使用的参考图；不为普通实物镜头或每个10秒段强制加图。若出现猫，另附三视图锁定身份；纯原理图不必出现猫。

```text
Create ONE mechanism reference frame for storyboard shot {shot_id}, {aspect_ratio}.
Image 1 is the ACTUAL PROP / STRUCTURE reference from this episode, not merely a mood reference.
Represent this exact object and region: {object, physical region, viewing/cut plane or magnified area}.
Preserve these recognition landmarks and relationships: {outline, key parts, contact surface, orientation, sealed versus open regions}.
The diagram depicts the SAME causal state as the real object at {time/state}. Internal change: {mechanism}. Corresponding external result: {result}.
Use {matching 3D cutaway or clear matched 2D/2.5D schematic}. Simplify only {nonessential textures/details}; never alter {causally important structure}.
The cutaway/transparent region is a viewing device, not a real opening, tear or new flow channel. Retain a readable relation to the original silhouette and contact points.
Symbols, only if needed: {what each particle/arrow means, its origin, direction, target and change}. Distinguish material flow from force. Do not pass material through an intact barrier or invent numbers.
No unrelated apparatus, decorative arrows, extra parts, long text, captions, cover title or watermark. One frame, not a montage. Scientific structure takes priority over visual spectacle.
```

检查轮廓和部位是否能与实物对应，内外、接触及通道是否正确，符号是否表达指定含义；图像对应通过不代表视频里的连续变化已经正确。记录实际参考图路径和用途，将生成图片与提示词保存在本期目录，必要时更新对应分镜与视频提示词。

## 实际修订

先检查生成图片再写下一步的编辑提示词。若图像工具未遵守姿势或器材状态，直接针对该问题编辑；不能只在文字里声称已纠正。修字仍用图像编辑，未经用户确认不转用Python绘图。
