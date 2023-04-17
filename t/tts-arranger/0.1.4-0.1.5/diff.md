# Comparing `tmp/tts_arranger-0.1.4.tar.gz` & `tmp/tts_arranger-0.1.5.tar.gz`

## Comparing `tts_arranger-0.1.4.tar` & `tts_arranger-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/requirements.txt
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/__init__.py
--rw-r--r--   0        0        0    25903 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/tts_processor.py
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/tts_processor_example.py
--rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/tts_simple_writer.py
--rw-r--r--   0        0        0    15511 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/tts_writer.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/data/replace.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/data/replace_de.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/data/replace_en.json
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/items/__init__.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/items/tts_chapter.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/items/tts_item.py
--rw-r--r--   0        0        0     5449 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/items/tts_project.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/utils/__init__.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/utils/audio.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/utils/log.py
--rw-r--r--   0        0        0    18265 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/tests/tts_arranger_test.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/LICENSE
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/README.md
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tts_arranger-0.1.5/requirements.txt
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tts_arranger-0.1.5/src/tts_arranger/__init__.py
+-rw-r--r--   0        0        0    24724 2020-02-02 00:00:00.000000 tts_arranger-0.1.5/src/tts_arranger/tts_processor.py
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 tts_arranger-0.1.5/src/tts_arranger/tts_processor_example.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 tts_arranger-0.1.5/src/tts_arranger/tts_simple_writer.py
+-rw-r--r--   0        0        0    15578 2020-02-02 00:00:00.000000 tts_arranger-0.1.5/src/tts_arranger/tts_writer.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 tts_arranger-0.1.5/src/tts_arranger/data/replace.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tts_arranger-0.1.5/src/tts_arranger/data/replace_de.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tts_arranger-0.1.5/src/tts_arranger/data/replace_en.json
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tts_arranger-0.1.5/src/tts_arranger/items/__init__.py
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 tts_arranger-0.1.5/src/tts_arranger/items/tts_chapter.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 tts_arranger-0.1.5/src/tts_arranger/items/tts_item.py
+-rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 tts_arranger-0.1.5/src/tts_arranger/items/tts_project.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.1.5/src/tts_arranger/utils/__init__.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 tts_arranger-0.1.5/src/tts_arranger/utils/audio.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 tts_arranger-0.1.5/src/tts_arranger/utils/log.py
+-rw-r--r--   0        0        0    20461 2020-02-02 00:00:00.000000 tts_arranger-0.1.5/tests/tts_arranger_test.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 tts_arranger-0.1.5/README.md
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 tts_arranger-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 tts_arranger-0.1.5/PKG-INFO
```

### Comparing `tts_arranger-0.1.4/src/tts_arranger/tts_processor.py` & `tts_arranger-0.1.5/src/tts_arranger/tts_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from pydub import AudioSegment  # type: ignore
 from pydub.silence import detect_silence  # type: ignore
 from TTS.utils.manage import ModelManager  # type: ignore
 from TTS.utils.synthesizer import Synthesizer  # type: ignore
 
 from .items.tts_item import TTS_Item
 from .utils.audio import numpy_to_segment
-from .utils.log import LOG_TYPE, log
+from .utils.log import LOG_TYPE, bcolors, log
 
 
 class TTS_Processor:
     def __init__(self, model='', vocoder: str = '', preferred_speakers: Optional[list[str]] = None) -> None:
         """
         Initializes a new instance of the TTS class.
 
@@ -85,15 +85,15 @@
 
     def initialize(self) -> None:
         """
         Initializes the text-to-speech (TTS) system, downloads the specified models, and populates the speaker list.
 
         :return: None
         """
-        log(LOG_TYPE.INFO, f'Initializing speech synthesizer')
+        log(LOG_TYPE.INFO, f'Initializing speech synthesizer.')
         models_dir = Path(TTS.__file__).resolve().parent / '.models.json'
         self.manager = ModelManager(str(models_dir))
 
         with contextlib.redirect_stdout(None):
             (model_path, config_path, _), (vocoder_path, vocoder_config_path, _) = [
                 self.manager.download_model(m) if m else ('', '', '') for m in (self.model, self.vocoder)
             ]
@@ -263,15 +263,15 @@
                     if match:
                         matched_text = match.group(0)
                         if len(matched_text) > 2:
                             first_char = matched_text[0]
                             text = re.sub(regex, first_char, text)
 
                     # Strip starting punctuation and normalize ending punctuation
-                    text = text.strip().lstrip(string.punctuation).strip()
+                    text = text.lstrip(string.punctuation)
 
                     if self.model != 'tts_models/en/vctk/vits':
                         # Add a full stop if necessary to avoid synthesizing problems with some models
                         text = re.sub(r'([a-zA-Z0-9])$', r'\1.', text)
 
                 if len(text) > 0:
                     if re.search(r'[a-zA-Z0-9]', text):
@@ -338,15 +338,15 @@
                         # From last group to end of current group
                         final_items.append(TTS_Item(item_text, tts_item.speaker, tts_item.speaker_idx, tts_item.length))
                         if pause_post_ms > 0:
                             final_items.append(TTS_Item(length=pause_post_ms))
                         last_start = m.end()
 
                 # From end of last group to end of text
-                text = text[last_start:].strip()
+                text = text[last_start:]
 
                 if text:
                     final_items.append(TTS_Item(text, tts_item.speaker, tts_item.speaker_idx, tts_item.length))
 
         return final_items
 
     def _get_character(self, text: str, pos: int) -> str:
@@ -402,15 +402,15 @@
                 if not tts_item.text and tts_item.length > 0:
                     final_items.append(tts_item)
 
                 # print(f'New item: {tts_item.text} / {tts_item.speaker}')
 
                 for idx, c in enumerate(tts_item.text):
                     new_item = copy.copy(tts_item)
-                    new_item.text = tts_item.text[pos:idx].strip()
+                    new_item.text = tts_item.text[pos:idx]
                     new_item.speaker = tts_item.speaker
                     current_speaker = tts_item.speaker
                     current_speaker_idx = tts_item.speaker_idx
 
                     add_item = False
 
                     # print(f'idx: {idx}')
@@ -474,15 +474,15 @@
 
                 if found:
                     if pause_post_ms > 0:
                         final_items.append(TTS_Item(length=pause_post_ms))
 
                 # Add rest / regular item
                 new_item = copy.copy(tts_item)
-                new_item.text = tts_item.text[pos:].strip()
+                new_item.text = tts_item.text[pos:]
                 new_item.speaker = current_speaker
                 new_item.speaker_idx = current_speaker_idx
                 new_item.length = tts_item.length
 
                 if new_item.text:
                     # print(f'Adding regular item: {new_item.text} / {new_item.speaker}')
                     final_items.append(new_item)
@@ -495,56 +495,19 @@
 
         :param tts_items: A list of TTS items to be preprocessed.
         :type tts_items: list[TTS_Item]
 
         :return: A new list of preprocessed TTS items.
         :rtype: list[TTS_Item]
         """
-        final_items = []
-        merged_items = self._merge_similar_items(tts_items)
-
-        for tts_item in merged_items:
-            final_items += self._prepare_item(tts_item)
-
-        return final_items
-
-    def _merge_similar_items(self, items: list[TTS_Item]) -> list[TTS_Item]:
-        """
-        Merge similar items for smoother synthesizing and avoiding unwanted pauses
-
-        :param items: A list of TTS items to merge
-        :type items: list
-
-        :return: A list of merged TTS items
-        :rtype: list[TTS_Item]
-        """
 
         final_items: list[TTS_Item] = []
-        merged_item: Optional[TTS_Item] = None
 
-        if items:
-            for item in items:
-                if not merged_item:
-                    # Scanning not started
-                    merged_item = item
-                elif merged_item.speaker == item.speaker and merged_item.speaker_idx == item.speaker_idx:
-                    # Starting item and current are similar, add to merge item text and length
-                    merged_item = merged_item.__class__(
-                        text=f'{merged_item.text}{item.text}',
-                        speaker=merged_item.speaker,
-                        speaker_idx=merged_item.speaker_idx,
-                        length=merged_item.length + item.length
-                    )
-                else:
-                    # Starting item and current are not similar, add last and current item, set this item as new starting item
-                    final_items.append(merged_item)
-                    merged_item = item
-
-            if merged_item is not None:
-                final_items.append(merged_item)
+        for tts_item in tts_items:
+            final_items += self._prepare_item(tts_item)
 
         return final_items
 
     def synthesize_tts_item(self, tts_item: TTS_Item) -> AudioSegment:
         """
         Synthesize a single item and return a PyDub AudioSegment object
 
@@ -560,22 +523,30 @@
             try:
                 speaker = ''
 
                 if self.synthesizer.tts_model and self.synthesizer.tts_model.num_speakers > 1:
                     speaker = tts_item.speaker or self.speakers[tts_item.speaker_idx % len(self.speakers)]
                     speaker = self.preferred_speakers[tts_item.speaker_idx % len(self.preferred_speakers)] if self.preferred_speakers and speaker in self.speakers else speaker
 
+                # Add a symbol to mark if not speaker was specified and it was derived from the speaker index
+                speaker_mark = ''
+
+                if not tts_item.speaker:
+                    speaker_mark = '*'
+
+                log(LOG_TYPE.INFO, f'("{speaker}"{speaker_mark}, {tts_item.speaker_idx}, {tts_item.length}ms):{bcolors.ENDC} {tts_item.text}')
+
                 # Suppress tts output
                 with contextlib.redirect_stdout(None):
                     wav = self.synthesizer.tts(
                         text=tts_item.text,
                         speaker_name=speaker,
                     )
             except Exception as e:
-                raise Exception(f'Error synthesizing "{tts_item.text}: {e}"')
+                raise Exception(f'Error synthesizing "{tts_item.text}: {e}".')
             else:
                 speech_segment = numpy_to_segment(np.array(wav), int(self.synthesizer.output_sample_rate))
 
                 # If length is predefined, add padding if necessary
                 if int(speech_segment.duration_seconds * 1000) < tts_item.length:
                     speech_segment += AudioSegment.silent(int(tts_item.length - speech_segment.duration_seconds * 1000), int(self.synthesizer.output_sample_rate))
                 else:
```

### Comparing `tts_arranger-0.1.4/src/tts_arranger/tts_processor_example.py` & `tts_arranger-0.1.5/src/tts_arranger/tts_processor_example.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.4/src/tts_arranger/tts_simple_writer.py` & `tts_arranger-0.1.5/src/tts_arranger/tts_simple_writer.py`

 * *Files 13% similar despite different names*

```diff
@@ -49,21 +49,20 @@
         for tts_item in tts_items:
             characters_sum += len(tts_item.text)
 
         segments = AudioSegment.empty()
 
         for idx, tts_item in enumerate(tts_items):
             if tts_item.text:
-                speaker = tts_item.speaker or self.preferred_speakers[tts_item.speaker_idx]
-                log(LOG_TYPE.INFO, f'Synthesizing item {idx + 1} of {len(tts_items)} "({speaker}", {tts_item.speaker_idx}, {tts_item.length}ms):{bcolors.ENDC} {tts_item.text}')
+                log(LOG_TYPE.INFO, f'Synthesizing item {idx + 1} of {len(tts_items)}:{bcolors.ENDC}')
             else:
-                log(LOG_TYPE.INFO, f'Adding pause: {tts_item.length}ms:{bcolors.ENDC} {tts_item.text}')
+                log(LOG_TYPE.INFO, f'Adding pause: {tts_item.length}ms:{bcolors.ENDC}')
 
             if time_needed:
-                log(LOG_TYPE.INFO, f'(Remaining time: {str(datetime.timedelta(seconds=round(time_needed)))})')
+                log(LOG_TYPE.INFO, f'(Remaining time: {str(datetime.timedelta(seconds=round(time_needed)))}).')
 
             time_last = time.time()
 
             try:
                 segments += tts_processor.synthesize_tts_item(tts_item)
 
                 time_now = time.time()
@@ -78,19 +77,19 @@
                 #     callback(idx, len(tts_items))
             except KeyboardInterrupt:
                 log(LOG_TYPE.ERROR, 'Stopped by user.')
                 sys.exit()
             except Exception as e:
                 # with open(self.temp_dir.name + '/tts-error.log', 'a+') as f:
                 #     f.write(f'Error synthesizing "{output_filename}"\n')
-                log(LOG_TYPE.ERROR, f'Error synthesizing "{output_filename}": {e}')
+                log(LOG_TYPE.ERROR, f'Error synthesizing "{output_filename}": {e}.')
                 sys.exit()
 
         self._write(segments, output_filename)
-        log(LOG_TYPE.SUCCESS, f'Synthesizing finished, file saved as {output_filename}')
+        log(LOG_TYPE.SUCCESS, f'Synthesizing finished, file saved as "{output_filename}".')
 
     def _write(self, segment: AudioSegment, output_filename: str) -> None:
         """
         Compress, convert and write AudioSegment as a given output file path and name
 
         :param segment: AudioSegment to be written
         :type segment: AudioSegment
@@ -111,15 +110,15 @@
         folder = os.path.dirname(os.path.abspath(output_filename))
 
         os.makedirs(folder, exist_ok=True)
 
         # Ensure output file name has a file extension
         output_filename = os.path.splitext(output_filename)[0] + '.' + format
 
-        log(LOG_TYPE.INFO, f'Compressing, converting and saving as {output_filename}')
+        log(LOG_TYPE.INFO, f'Compressing, converting and saving as {output_filename}.')
 
         comp_expansion = 12.5
         comp_raise = 0.0001
 
         # Apply dynamic compression
         # segment.export(output_filename, format, parameters=['-filter', 'speechnorm=e=25:r=0.0001:l=1', '-filter', 'loudnorm=tp=-1.0:offset=7'])
         params = ['-filter', f'speechnorm=e={comp_expansion}:r={comp_raise}:l=1']
```

### Comparing `tts_arranger-0.1.4/src/tts_arranger/tts_writer.py` & `tts_arranger-0.1.5/src/tts_arranger/tts_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
         :return: The duration of the audio file in nanoseconds.
         :rtype: int
         """
         result = ffmpeg.probe(file_name, cmd='ffprobe', show_entries='format=duration')
         return int(float(result['format']['duration']) * self.NANOSECONDS_IN_ONE_SECOND)
 
-    def _synthesize_chapters(self, chapters: list[TTS_Chapter], temp_dir: str, tts_processor: TTS_Processor, callback: Callable[[float, TTS_Item], None] | None = None) -> None:
+    def _synthesize_chapters(self, chapters: list[TTS_Chapter], temp_dir: str, tts_processor: TTS_Processor, callback: Callable[[float, TTS_Item], None] | None = None, max_pause_duration=0) -> None:
         """
         Private method for synthesizing chapters into audio.
 
         :param chapters: A list of TTS chapters containing text to be synthesized into audio.
         :type chapters: list[TTS_Chapter]
 
         :param temp_dir: Path to the temporary directory.
@@ -84,18 +84,19 @@
         :param callback: An optional function that can be used to monitor the progress of the synthesis process.
         :type callback: Callable[[float, TTS_Item], None] | None
 
         :return: None
         :rtype: None
         """
 
-        log(LOG_TYPE.INFO, f'Preprocessing items')
+        log(LOG_TYPE.INFO, f'Preprocessing items.')
 
         for chapter in chapters:
             chapter.tts_items = tts_processor.preprocess_items(chapter.tts_items)
+            chapter.optimize(max_pause_duration)
 
         tts_processor.initialize()
 
         total_items = 0
 
         for chapter in chapters:
             total_items += len(chapter.tts_items)
@@ -108,39 +109,40 @@
             audio = AudioSegment.empty()
 
             temp_format = 'wav'
 
             filename = os.path.join(temp_dir, f'tts_part_{i}.{temp_format}')
 
             if len(chapters) > 1:
-                log(LOG_TYPE.INFO, f'Synthesizing chapter {i + 1} of {len(chapters)}')
+                log(LOG_TYPE.INFO, f'Synthesizing chapter {i + 1} of {len(chapters)}.')
 
             if len(chapter.tts_items) > 0:
                 for j, tts_item in enumerate(chapter.tts_items):
                     if tts_item.text:
-                        speaker = tts_item.speaker or self.preferred_speakers[tts_item.speaker_idx]
-                        log(LOG_TYPE.INFO, f'Synthesizing item {j + 1} of {len(chapter.tts_items)} ("{speaker}", {tts_item.speaker_idx}, {tts_item.length}ms):{bcolors.ENDC} {tts_item.text}')
+                        log(LOG_TYPE.INFO, f'Synthesizing item {j + 1} of {len(chapter.tts_items)}:{bcolors.ENDC}')
                     else:
-                        log(LOG_TYPE.INFO, f'Adding pause: {tts_item.length}ms:{bcolors.ENDC} {tts_item.text}')
+                        log(LOG_TYPE.INFO, f'Adding pause: {tts_item.length}ms:{bcolors.ENDC}')
 
+                    # Synthesize audio from TTS item text
                     audio += tts_processor.synthesize_tts_item(tts_item)
 
                     if callback is not None:
                         callback(100/(len(chapters) * len(chapter.tts_items)) * (i + j), tts_item)
 
-                current_total_items += len(chapter.tts_items)
-
+                # Write synthesized audio as temp file
                 self._write_temp_audio(audio, filename)
 
+                current_total_items += len(chapter.tts_items)
+
                 num_zeros = len(str(len(self.temp_files)))
                 chapter_title = f'{i + 1:0{num_zeros}} - {chapter.title}'
 
                 filename_out = os.path.join(temp_dir, f'tts_part_{i}.{temp_format}')
 
-                # Add temp files for concatenating later
+                # Add temp file for concatenating later
                 self.temp_files.append((chapter_title, filename_out))
 
             chapter.start_time = cumulative_time
             chapter.end_time = cumulative_time + self._get_nanoseconds_for_file(filename)
             cumulative_time = chapter.end_time
 
         del tts_processor
@@ -226,15 +228,15 @@
 
         # Apply dynamic compression
         params = ['-filter', f'speechnorm=e={comp_expansion}:r={comp_raise}:l=1']
         bitrate = '320k'
         format = 'wav'
         segment.export(output_filename, format, parameters=params, bitrate=bitrate)
 
-    def synthesize_and_write(self, project_filename: str, temp_dir_prefix: str = '', concat=True, callback: Callable[[float, TTS_Item], None] | None = None) -> None:
+    def synthesize_and_write(self, project_filename: str, temp_dir_prefix: str = '', concat=True, callback: Callable[[float, TTS_Item], None] | None = None, max_pause_duration=0) -> None:
         """
         Synthesize and write the output audio files for the given project.
 
         :param project_filename: The project name.
         :type project_filename: str
 
         :param temp_dir_prefix: An optional prefix for the temporary directory name used during synthesis.
@@ -248,40 +250,40 @@
 
         :return: None
 
         :raises: ValueError if `project_filename` is not a valid file path.
         """
 
         if not self.project.tts_chapters:
-            log(LOG_TYPE.ERROR, f'No chapters to synthesize, exiting')
+            log(LOG_TYPE.ERROR, f'No chapters to synthesize, exiting.')
             return
 
         with tempfile.TemporaryDirectory(prefix=temp_dir_prefix) as temp_dir:
             try:
-                log(LOG_TYPE.INFO, f'Synthesizing {self.project.title}')
+                log(LOG_TYPE.INFO, f'Synthesizing project "{self.project.title}".')
 
                 if self.model and self.vocoder:
                     t = TTS_Processor(self.model, self.vocoder, self.preferred_speakers)
                 else:
                     match self.project.lang_code:
                         case 'en':
                             self.model = 'tts_models/en/vctk/vits'
                             self.vocoder = ''
                         case 'de':
                             self.model = 'tts_models/de/thorsten/tacotron2-DDC'
                             self.vocoder = 'vocoder_models/de/thorsten/hifigan_v1'
                         case _:
-                            raise ValueError(f'Language code {self.project.lang_code} not supported')
+                            raise ValueError(f'Language code "{self.project.lang_code}" not supported')
 
                     t = TTS_Processor(self.model, self.vocoder, self.preferred_speakers)
 
-                self._synthesize_chapters(self.project.tts_chapters, temp_dir, t, callback)
+                self._synthesize_chapters(self.project.tts_chapters, temp_dir, t, callback, max_pause_duration)
 
             except Exception as e:
-                log(LOG_TYPE.ERROR, f'Synthesizing {self.project.title} failed: {e}')
+                log(LOG_TYPE.ERROR, f'Synthesizing project "{self.project.title}" failed: {e}.')
                 sys.exit(1)
 
             finally:
                 # Prepare chapter metadata
                 metadata_lines = [';FFMETADATA1\n']
 
                 for chapter in self.project.tts_chapters:
@@ -324,15 +326,15 @@
 
                     # Remove last map parameter (workaround for ffmpeg-python bug)
                     cmd = self._remove_last_arg(cmd, '-map')
 
                     subprocess.call(cmd)
 
                     output_files.append(output_path)
-                    log(LOG_TYPE.SUCCESS, f'Synthesizing project {self.project.title} finished, file saved as {output_path}')
+                    log(LOG_TYPE.SUCCESS, f'Synthesizing project {self.project.title} finished, file saved as "{output_path}".')
                 else:
                     # Don’t concatenate, convert the chapter temp files to the target format
                     os.makedirs(output_filename, exist_ok=True)
 
                     for name, file in self.temp_files:
                         output_chapter_filename = os.path.join(output_filename, name + output_extension)
 
@@ -346,15 +348,15 @@
                             ffmpeg
                             .input(file)
                             .output(output_chapter_filename, **output_args, loglevel='error')
                             .run(overwrite_output=True)
                         )
 
                         output_files.append(output_chapter_filename)
-                    log(LOG_TYPE.SUCCESS, f'Synthesizing project {self.project.title} finished, chapter files saved under {output_filename}/')
+                    log(LOG_TYPE.SUCCESS, f'Synthesizing project {self.project.title} finished, chapter files saved under "{output_filename}/".')
 
                 if self.project.image_bytes:
                     if self.output_format in ['m4b', 'm4a', 'mp3']:
                         image_bytes = base64.b64decode(self.project.image_bytes)
                         image_file = io.BytesIO(image_bytes)
                         image = Image.open(image_file)
```

### Comparing `tts_arranger-0.1.4/src/tts_arranger/items/tts_item.py` & `tts_arranger-0.1.5/src/tts_arranger/items/tts_item.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.4/src/tts_arranger/items/tts_project.py` & `tts_arranger-0.1.5/src/tts_arranger/items/tts_project.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import base64
 import datetime
 from io import BytesIO
 import pickle
 from dataclasses import dataclass, field
+from typing import Optional
 from PIL import Image
 
 
 import requests  # type: ignore
 
 from ..utils.log import LOG_TYPE, log
 from .tts_chapter import TTS_Chapter  # type: ignore
@@ -64,28 +65,41 @@
             try:
                 with open(filename, 'rb') as file:
                     return pickle.load(file)
             except IOError:
                 log(LOG_TYPE.WARNING, f'TTS Project export file "{filename}" could not be opened for reading.')
         return TTS_Project()
 
+    @classmethod
+    def from_items(cls, tts_items: list[TTS_Item]):
+        """
+        Convenience method to create a TTS project from a list of TTS items.
+
+        :param filename: A list with TTS item to create TTS project from (containing a single chapter containing the items).
+        :type filename: str
+
+        :return: A TTS project object loaded from the JSON file.
+        :rtype: TTS_Project
+        """
+        return TTS_Project([TTS_Chapter(tts_items)])
+
     def merge_from_project(self, project) -> None:
         """
         Method to merge the contents of another TTS project into this one.
 
         :param project: The TTS project to be merged.
         :type project: TTS_Project
 
         :return: None
         :rtype: None
         """
         if isinstance(project, TTS_Project):
             self.tts_chapters += project.tts_chapters
 
-    def add(self, items: list[TTS_Item]) -> None:
+    def append(self, items: list[TTS_Item]) -> None:
         """
         Method to add a list of TTS items to the last TTS chapter of this TTS project.
 
         :param items: A list of TTS items to be added to the last chapter.
         :type items: list[TTS_Item]
 
         :return: None
@@ -95,15 +109,15 @@
         if not self.tts_chapters:
             self.tts_chapters.append(TTS_Chapter())
 
         self.tts_chapters[-1].tts_items += items
 
     def to_json_file(self, filename: str) -> None:
         """
-        Method to save this TTS project to a JSON file.
+        Method to save the TTS project to a JSON file.
 
         :param filename: A string representing the name of the JSON file to be saved.
         :type filename: str
 
         :return: None
         :rtype: None
         """
@@ -165,7 +179,20 @@
         final_chapters: list[TTS_Chapter] = []
 
         for chapter in self.tts_chapters:
             if len(chapter.tts_items) > 0:
                 final_chapters.append(chapter)
 
         self.tts_chapters = final_chapters
+
+    def optimize(self, max_pause_duration=0) -> None:
+        """
+        Merge similar items for smoother synthesizing and avoiding unwanted pauses
+
+        :param max_pause_duration: Maximum duration auf merged pauses
+        :type max_pause_duration: int
+
+        :return: None
+        """
+
+        for chapter in self.tts_chapters:
+            chapter.optimize(max_pause_duration)
```

### Comparing `tts_arranger-0.1.4/src/tts_arranger/utils/audio.py` & `tts_arranger-0.1.5/src/tts_arranger/utils/audio.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.4/src/tts_arranger/utils/log.py` & `tts_arranger-0.1.5/src/tts_arranger/utils/log.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.4/tests/tts_arranger_test.py` & `tts_arranger-0.1.5/tests/tts_arranger_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,30 +90,30 @@
 
     def test_punctuation2(self):
         t = TTS_Processor()
 
         tts_item = TTS_Item('Specifically, he wanted to bring FORTRAN, as it happens the implementation language of the original Adventure (not that Ken likely knew this or cared), to the little Apple II.', '')
 
         tts_items = t._prepare_item(tts_item)
-        self.assertEqual(tts_items[0].text, 'Specifically, he wanted to bring FORTRAN, as it happens the implementation language of the original Adventure')
+        self.assertEqual(tts_items[0].text, 'Specifically, he wanted to bring FORTRAN, as it happens the implementation language of the original Adventure ')
         self.assertEqual(tts_items[1].length, 300)
         self.assertEqual(tts_items[2].text, 'not that Ken likely knew this or cared,')
         self.assertEqual(tts_items[3].length, 300)
-        self.assertEqual(tts_items[4].text, 'to the little Apple 2.')
+        self.assertEqual(tts_items[4].text, ' to the little Apple 2.')
         self.assertEqual(tts_items[5].length, 750)
 
     def test_punctuation3(self):
         t = TTS_Processor()
 
         tts_item = TTS_Item('a — b.', '')
 
         tts_items = t._prepare_item(tts_item)
-        self.assertEqual(tts_items[0].text, 'a')
+        self.assertEqual(tts_items[0].text, 'a ')
         self.assertEqual(tts_items[1].length, 300)
-        self.assertEqual(tts_items[2].text, 'b.')
+        self.assertEqual(tts_items[2].text, ' b.')
         self.assertEqual(tts_items[3].length, 750)
 
     # def test_punctuation3(self):
     #     t = TTS_Arranger()
 
     #     tts_item = TTS_Item('Much of what led to designs like The Wizard and the Princess — the lack of understood “best practices” for game design, primitive technology, the simple inexperience of the designers themselves — I’ve already mentioned here and elsewhere. Certainly, as I’ve particularly harped, it was difficult with a Scott Adams- or Hi-Res-Adventures-level parser and world model to find a ground for challenging puzzles that were not unfair; the leap from trivial to impossible being made in one seemingly innocuous hop, as it were.', '')
 
@@ -343,7 +343,72 @@
             output_file_path = os.path.join(output_dir, f'{project.author} - {project.title}.{output_format}')
 
             # Ensure that the output file was created
             self.assertTrue(os.path.exists(output_file_path))
 
             # Ensure that the output file has a non-zero size
             self.assertGreater(os.path.getsize(output_file_path), 0)
+
+    def test_merge_items1(self):
+        items = []
+        items.append(TTS_Item('1 '))
+        items.append(TTS_Item('2'))
+        items.append(TTS_Item(' 3'))
+
+        project = TTS_Project()
+        project.tts_chapters.append(TTS_Chapter(items))
+        project.optimize()
+        items = project.tts_chapters[0].tts_items
+
+        self.assertEqual(items[0].text, '1 2 3')
+
+    def test_merge_items2(self):
+        items = []
+        items.append(TTS_Item('1 '))
+        items.append(TTS_Item(length=1000))
+        items.append(TTS_Item('2'))
+        items.append(TTS_Item(length=1000))
+        items.append(TTS_Item(' 3'))
+
+        project = TTS_Project()
+        project.tts_chapters.append(TTS_Chapter(items))
+        project.optimize()
+        items = project.tts_chapters[0].tts_items
+
+        self.assertEqual(items[0].text, '1 ')
+        self.assertEqual(items[1].length, 1000)
+        self.assertEqual(items[2].text, '2')
+        self.assertEqual(items[3].length, 1000)
+        self.assertEqual(items[4].text, ' 3')
+
+    def test_merge_items3(self):
+        items = []
+        items.append(TTS_Item('1 '))
+        items.append(TTS_Item('2'))
+        items.append(TTS_Item(length=1000))
+        items.append(TTS_Item(length=1000))
+        items.append(TTS_Item(' 3'))
+        items.append(TTS_Item(length=1000))
+
+        project = TTS_Project()
+        project.tts_chapters.append(TTS_Chapter(items))
+        project.optimize(max_pause_duration=100)
+        items = project.tts_chapters[0].tts_items
+
+        self.assertEqual(items[0].text, '1 2')
+        self.assertEqual(items[1].length, 100)
+        self.assertEqual(items[2].text, ' 3')
+        self.assertEqual(items[3].length, 100)
+
+    def test_merge_items4(self):
+        item = TTS_Item('1 (1234), test')
+        t = TTS_Processor()
+        tts_items = t._prepare_item(item)
+        
+        project = TTS_Project()
+        project.tts_chapters.append(TTS_Chapter(tts_items))
+        project.optimize(max_pause_duration=100)
+        items = project.tts_chapters[0].tts_items
+
+        self.assertEqual(items[0].text, '1 ')
+        self.assertEqual(items[2].text, '1234,')
+        self.assertEqual(items[4].text, ' test')
```

### Comparing `tts_arranger-0.1.4/LICENSE` & `tts_arranger-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.4/README.md` & `tts_arranger-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.4/pyproject.toml` & `tts_arranger-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   "Operating System :: OS Independent",
 ]
 description = "Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS"
 dynamic = ["dependencies"]
 name = "tts_arranger"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "0.1.4"
+version = "0.1.5"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/knochenhans/tts_arranger/issues"
 "Homepage" = "https://github.com/knochenhans/tts_arranger"
 
 [tool.hatch.build]
 exclude = [
```

### Comparing `tts_arranger-0.1.4/PKG-INFO` & `tts_arranger-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tts_arranger
-Version: 0.1.4
+Version: 0.1.5
 Summary: Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS
 Project-URL: Bug Tracker, https://github.com/knochenhans/tts_arranger/issues
 Project-URL: Homepage, https://github.com/knochenhans/tts_arranger
 Author-email: Andre Jonas <nipsky@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

