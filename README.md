# Rotary Encoder for STM32


Invoke Like this:

```c
	ROTARY_ENCODER_CONFIG encoder_configs[2];
	encoder_configs[0].switch_bus = GPIOA;
	encoder_configs[0].switch_idx = GPIO_PIN_0;
	encoder_configs[0].pin_a_bus = GPIOA;
	encoder_configs[0].pin_a_idx = GPIO_PIN_2;
	encoder_configs[0].pin_b_bus = GPIOA;
	encoder_configs[0].pin_b_idx = GPIO_PIN_1;	
	encoder_configs[0].parameter = CURRENT;

	encoder_configs[1].switch_bus = GPIOC;
	encoder_configs[1].switch_idx = GPIO_PIN_13;
	encoder_configs[1].pin_a_bus = GPIOC;
	encoder_configs[1].pin_a_idx = GPIO_PIN_14;
	encoder_configs[1].pin_b_bus = GPIOC;
	encoder_configs[1].pin_b_idx = GPIO_PIN_15;
	encoder_configs[1].parameter = VOLTAGE;

	ROTARY_ENCODER.configure(encoder_configs, 2);

```
