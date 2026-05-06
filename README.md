# --- THE NEW BUILT-IN VOICE NOTES ---
st.subheader(text["notes"])

# This adds a native microphone widget
audio_value = st.audio_input(text["mic"])

if audio_value:
    # This displays the audio so you can listen back to your notes
    st.audio(audio_value)
    st.info("Audio note recorded! Listen back above.")

# Standard text area for manual notes
notes = st.text_area("Manual Notes", height=100, label_visibility="collapsed")
