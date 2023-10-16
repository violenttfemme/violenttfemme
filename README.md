import keyboard

def main():
    print("Presiona la tecla ↑ para detener el bucle.")
    
    while True:
        event = keyboard.read_event(suppress=True)
        
        if event.event_type == keyboard.KEY_DOWN:
            if event.name == "up":
                print("Deteniendo el bucle.")
                break
            else:
                print(f"Tecla presionada: {event.name}")

if _name_ == "_main_":
    main()
