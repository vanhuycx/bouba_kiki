
function new_timeline() {
  var timeline = [];
  
  // manually preload these files, since not on standard jspsych preload
  var audio = ['sound/up2.wav'];
  
  var preload = {
    type: 'preload',
    auto_preload: true,  // automatic preload of stimulus files
    audio: audio  // manual preload of other files
  };


  var instruction = {
    type: 'html-button-response',
    stimulus: '<div style="max-width:600px;"><p>Instruction:</p> <p>An image of two random objects will be showed on the screen. You will hear an audio sound. Next, you will select the object that you think is associated with the sound. On the keyboard, clicking the left "Shift" button to select the left image and the right "Shift" button to select the right image.</p></div>',
    choices: ['Continue'],
   on_start: function() {
        // set progress bar to 0 at the start of experiment
       jsPsych.setProgressBar(0);
   }
  };
  
  var w = window.innerWidth;
  var h = window.innerHeight;
  
  var screen_size = {
    type: 'html-button-response',
    stimulus: '<p style="color: red; font-size: 20px"> Width: ' + w +' Height: ' + h  +'</p>',
    choices: ['Continue'],
  };
  
  
  var stimuli_arrays = 
  [
  
    [
      { stimulus: 'sound/baba_rep.wav',imageLeft:'img/bouba_7_L_white.png',imageRight:"img/kiki_7_L_white.png"},
      /*{ stimulus: 'sound/teetee.wav',imageRight:'img/bouba_3_L_white.png',imageLeft:"img/kiki_3_L_white.png"},
      { stimulus: 'sound/teetee.wav',imageLeft:'img/bouba_7_S_white.png',imageRight:"img/kiki_7_S_white.png"},
      { stimulus: 'sound/gaga_rep.wav',imageRight:'img/bouba_7_L_white.png',imageLeft:"img/kiki_7_L_white.png"},
  
      { stimulus: 'sound/gaga_rep.wav',imageLeft:'img/bouba_3_S_white.png',imageRight:"img/kiki_3_S_white.png"},
      /*{ stimulus: 'sound/keekee.wav',imageLeft:'img/bouba_3_L_white.png',imageRight:"img/kiki_3_L_white.png"},
      { stimulus: 'sound/baba_rep.wav',imageRight:'img/bouba_3_L_white.png',imageLeft:"img/kiki_3_L_white.png"},
      { stimulus: 'sound/keekee.wav',imageRight:'img/bouba_3_S_white.png',imageLeft:"img/kiki_3_S_white.png"},
  
      { stimulus: 'sound/gaga_rep.wav',imageLeft:'img/bouba_3_L_white.png',imageRight:"img/kiki_3_L_white.png"},
      { stimulus: 'sound/teetee.wav',imageLeft:'img/bouba_3_S_white.png',imageRight:"img/kiki_3_S_white.png"},
      { stimulus: 'sound/baba_rep.wav',imageLeft:'img/bouba_3_S_white.png',imageRight:"img/kiki_3_S_white.png"},
      { stimulus: 'sound/keekee.wav',imageRight:'img/bouba_7_S_white.png',imageLeft:"img/kiki_7_S_white.png"},
  
      { stimulus: 'sound/teetee.wav',imageRight:'img/bouba_7_L_white.png',imageLeft:"img/kiki_7_L_white.png"},
      { stimulus: 'sound/keekee.wav',imageLeft:'img/bouba_7_L_white.png',imageRight:"img/kiki_7_L_white.png"},
      { stimulus: 'sound/gaga_rep.wav',imageRight:'img/bouba_7_S_white.png',imageLeft:"img/kiki_7_S_white.png"},
      { stimulus: 'sound/baba_rep.wav',imageRight:'img/bouba_7_S_white.png',imageLeft:"img/kiki_7_S_white.png"},
  
  
      { stimulus: 'sound/baba_rep.wav',imageRight:'img/bouba_7_L_white.png',imageLeft:"img/kiki_7_L_white.png"},
      { stimulus: 'sound/teetee.wav',imageLeft:'img/bouba_3_L_white.png',imageRight:"img/kiki_3_L_white.png"},
      { stimulus: 'sound/teetee.wav',imageRight:'img/bouba_7_S_white.png',imageLeft:"img/kiki_7_S_white.png"},
      { stimulus: 'sound/gaga_rep.wav',imageLeft:'img/bouba_7_L_white.png',imageRight:"img/kiki_7_L_white.png"},
  
      { stimulus: 'sound/gaga_rep.wav',imageRight:'img/bouba_3_S_white.png',imageLeft:"img/kiki_3_S_white.png"},
      { stimulus: 'sound/keekee.wav',imageRight:'img/bouba_3_L_white.png',imageLeft:"img/kiki_3_L_white.png"},
      { stimulus: 'sound/baba_rep.wav',imageLeft:'img/bouba_3_L_white.png',imageRight:"img/kiki_3_L_white.png"},
      { stimulus: 'sound/keekee.wav',imageLeft:'img/bouba_3_S_white.png',imageRight:"img/kiki_3_S_white.png"},
  
      { stimulus: 'sound/gaga_rep.wav',imageRight:'img/bouba_3_L_white.png',imageLeft:"img/kiki_3_L_white.png"},
      { stimulus: 'sound/teetee.wav',imageRight:'img/bouba_3_S_white.png',imageLeft:"img/kiki_3_S_white.png"},
      { stimulus: 'sound/baba_rep.wav',imageRight:'img/bouba_3_S_white.png',imageLeft:"img/kiki_3_S_white.png"},
      { stimulus: 'sound/keekee.wav',imageLeft:'img/bouba_7_S_white.png',imageRight:"img/kiki_7_S_white.png"},
  
      { stimulus: 'sound/teetee.wav',imageLeft:'img/bouba_7_L_white.png',imageRight:"img/kiki_7_L_white.png"},
      { stimulus: 'sound/keekee.wav',imageRight:'img/bouba_7_L_white.png',imageLeft:"img/kiki_7_L_white.png"},
      { stimulus: 'sound/gaga_rep.wav',imageLeft:'img/bouba_7_S_white.png',imageRight:"img/kiki_7_S_white.png"},
      { stimulus: 'sound/baba_rep.wav',imageLeft:'img/bouba_7_S_white.png',imageRight:"img/kiki_7_S_white.png"},
      
      */
    ],
    
    
    [
      { stimulus: 'sound/baba_rep.wav',imageLeft:'img/bouba_3_S_white.png',imageRight:"img/kiki_3_S_white.png"},
      /*{ stimulus: 'sound/teetee.wav',imageRight:'img/bouba_7_L_white.png',imageLeft:"img/kiki_7_L_white.png"},
      { stimulus: 'sound/gaga_rep.wav',imageRight:'img/bouba_3_S_white.png',imageLeft:"img/kiki_3_S_white.png"},
      { stimulus: 'sound/teetee.wav',imageLeft:'img/bouba_7_S_white.png',imageRight:"img/kiki_7_S_white.png"},
  
      { stimulus: 'sound/keekee.wav',imageLeft:'img/bouba_7_L_white.png',imageRight:"img/kiki_7_L_white.png"},
      { stimulus: 'sound/gaga_rep.wav',imageRight:'img/bouba_3_L_white.png',imageLeft:"img/kiki_3_L_white.png"},
      { stimulus: 'sound/gaga_rep.wav',imageLeft:'img/bouba_7_S_white.png',imageRight:"img/kiki_7_S_white.png"},
      { stimulus: 'sound/keekee.wav',imageRight:'img/bouba_3_S_white.png',imageLeft:"img/kiki_3_S_white.png"},
  
      { stimulus: 'sound/gaga_rep.wav',imageLeft:'img/bouba_7_L_white.png',imageRight:"img/kiki_7_L_white.png"},
      { stimulus: 'sound/baba_rep.wav',imageRight:'img/bouba_3_L_white.png',imageLeft:"img/kiki_3_L_white.png"},
      { stimulus: 'sound/keekee.wav',imageRight:'img/bouba_7_S_white.png',imageLeft:"img/kiki_7_S_white.png"},
      { stimulus: 'sound/baba_rep.wav',imageRight:'img/bouba_7_S_white.png',imageLeft:"img/kiki_7_S_white.png"},
  
      { stimulus: 'sound/teetee.wav',imageLeft:'img/bouba_3_L_white.png',imageRight:"img/kiki_3_L_white.png"},
      { stimulus: 'sound/teetee.wav',imageRight:'img/bouba_3_S_white.png',imageLeft:"img/kiki_3_S_white.png"},
      { stimulus: 'sound/keekee.wav',imageLeft:'img/bouba_3_L_white.png',imageRight:"img/kiki_3_L_white.png"},
      { stimulus: 'sound/baba_rep.wav',imageLeft:'img/bouba_7_L_white.png',imageRight:"img/kiki_7_L_white.png"},
  
  
  
      { stimulus: 'sound/baba_rep.wav',imageRight:'img/bouba_3_S_white.png',imageLeft:"img/kiki_3_S_white.png"},
      { stimulus: 'sound/teetee.wav',imageLeft:'img/bouba_7_L_white.png',imageRight:"img/kiki_7_L_white.png"},
      { stimulus: 'sound/gaga_rep.wav',imageLeft:'img/bouba_3_S_white.png',imageRight:"img/kiki_3_S_white.png"},
      { stimulus: 'sound/teetee.wav',imageRight:'img/bouba_7_S_white.png',imageLeft:"img/kiki_7_S_white.png"},
  
      { stimulus: 'sound/keekee.wav',imageRight:'img/bouba_7_L_white.png',imageLeft:"img/kiki_7_L_white.png"},
      { stimulus: 'sound/gaga_rep.wav',imageLeft:'img/bouba_3_L_white.png',imageRight:"img/kiki_3_L_white.png"},
      { stimulus: 'sound/gaga_rep.wav',imageRight:'img/bouba_7_S_white.png',imageLeft:"img/kiki_7_S_white.png"},
      { stimulus: 'sound/keekee.wav',imageLeft:'img/bouba_3_S_white.png',imageRight:"img/kiki_3_S_white.png"},
  
      { stimulus: 'sound/gaga_rep.wav',imageRight:'img/bouba_7_L_white.png',imageLeft:"img/kiki_7_L_white.png"},
      { stimulus: 'sound/baba_rep.wav',imageLeft:'img/bouba_3_L_white.png',imageRight:"img/kiki_3_L_white.png"},
      { stimulus: 'sound/keekee.wav',imageLeft:'img/bouba_7_S_white.png',imageRight:"img/kiki_7_S_white.png"},
      { stimulus: 'sound/baba_rep.wav',imageLeft:'img/bouba_7_S_white.png',imageRight:"img/kiki_7_S_white.png"},
  
      { stimulus: 'sound/teetee.wav',imageRight:'img/bouba_3_L_white.png',imageLeft:"img/kiki_3_L_white.png"},
      { stimulus: 'sound/teetee.wav',imageLeft:'img/bouba_3_S_white.png',imageRight:"img/kiki_3_S_white.png"},
      { stimulus: 'sound/keekee.wav',imageRight:'img/bouba_3_L_white.png',imageLeft:"img/kiki_3_L_white.png"},
      { stimulus: 'sound/baba_rep.wav',imageRight:'img/bouba_7_L_white.png',imageLeft:"img/kiki_7_L_white.png"},
      */
    ]
    
  ];
  
  
  // Pick a random array inside the stimuli_arrays
  
  var selected_array = stimuli_arrays[Math.floor(Math.random() * stimuli_arrays.length)];
  

  var n_trials = selected_array.length;

  var trial = {
    type: 'bouba-kiki',
    upsound: 'sound/up2.wav',
    choices: ['shiftleft','shiftright','escape'],
    stimulus: jsPsych.timelineVariable('stimulus'),
    image:[jsPsych.timelineVariable('imageLeft'),jsPsych.timelineVariable('imageRight')],
    data: {
      width: w,
      height: h,
      left_image: [jsPsych.timelineVariable('imageLeft')],
      right_image: [jsPsych.timelineVariable('imageRight')],
      
    },
    on_finish: function(data) {
        // at the end of each trial, update the progress bar
        // based on the current value and the proportion to update for each trial
        var curr_progress_bar_value = jsPsych.getProgressBarCompleted();
        jsPsych.setProgressBar(curr_progress_bar_value + (1/n_trials));
        
        
        // If 'escape' button is pressed, end the experiment and save the progress 
         if(jsPsych.pluginAPI.compareKeys(data.response, "escape")){
      jsPsych.endExperiment('The experiment was ended by pressing "escape".');
         }
    }
  };
  
  var loop_time = 1;
  
  var test_procedure = {
    timeline: [trial],
    timeline_variables: selected_array,
    loop_function: function (data) {
      var response_array = data.values();
      
      
      // Loop backward from the end. If the response is shiftleft or shiftright, splice out of the looped selected_array
      
     
      for (let i = response_array.length - 1; i >= 0; i--) {
        if ((response_array[i].response == "shiftleft") || (response_array[i].response == "shiftright")) {
          selected_array.splice(i, 1);
        }
      }
      

      // If the selected_array contains non_empty, execute the loop to resume wrong-key trial(s)
      if (loop_time == 1) {
        for (let i = 0; i < selected_array.length; i++) {
          if (selected_array[i]) {
            loop_time++;
            return true;
          }
        }
      } 
    

      return false;
    }
    
  };


  
  timeline.push(preload,instruction,test_procedure);


  return timeline;
}







